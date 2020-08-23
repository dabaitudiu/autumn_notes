## Socket范例
### Server
```java
package network;

import java.io.*;
import java.net.ServerSocket;
import java.net.Socket;

public class Server {
    public static void main(String[] args) {
        final int DEFAULT_PORT = 8888;
        final String QUIT = "QUIT";
        ServerSocket serverSocket = null;


        try {
            serverSocket = new ServerSocket(DEFAULT_PORT);
            while (true) {
                System.out.println("Listening on Port " + DEFAULT_PORT);
                Socket socket = serverSocket.accept();
                System.out.println("Client connection established: " + socket.getPort());

                BufferedReader reader = new BufferedReader(
                        new InputStreamReader(socket.getInputStream())
                );

                BufferedWriter writer = new BufferedWriter(
                        new OutputStreamWriter(socket.getOutputStream())
                );

                String msg = null;
                while ((msg = reader.readLine()) != null) {
                    System.out.println("Client[" + socket.getPort() + "]: " + msg);

                    writer.write("An add-on message to " + msg + "\n");
                    writer.flush();

                    if (msg.equals(QUIT)) {
                        System.out.println("Client[" + socket.getPort() + " has disconnected. " );
                        break;
                    }
                }
            }
        } catch (IOException e) {
            e.printStackTrace();
        } finally {
            if (serverSocket != null) {
                try {
                    serverSocket.close();
                } catch (IOException e) {
                    e.printStackTrace();
                }
            }
        }
    }
}

```

### Client
```java
package network;

import java.io.*;
import java.net.Socket;

public class Client {
    public static void main(String[] args) {
        final int DEFAULT_PORT = 8888;
        final String DEFAULT_SERVER_HOST = "127.0.0.1";
        final String QUIT = "QUIT";
        Socket socket = null;
        BufferedWriter writer = null;

        try {
            socket = new Socket(DEFAULT_SERVER_HOST,DEFAULT_PORT);

            BufferedReader reader = new BufferedReader(new InputStreamReader(socket.getInputStream()));
            writer = new BufferedWriter(new OutputStreamWriter(socket.getOutputStream()));

            BufferedReader consoleReader = new BufferedReader(new InputStreamReader(System.in));
            while (true) {
                String input = consoleReader.readLine();

                writer.write(input + "\n");
                writer.flush();

                String msg = reader.readLine();
                System.out.println("Message from host: " + msg);

                if (input.equals(QUIT)) {
                    break;
                }

            }

        } catch (IOException e) {
            e.printStackTrace();
        } finally {
            if (writer != null) {
                try {
                    writer.close();
                } catch (IOException e) {
                    e.printStackTrace();
                }
            }
        }

    }
}

```