# Video File Transfer Over TCP Sockets

This project involves designing and coding a sender/receiver program to transmit video file contents over TCP sockets with a graphical user interface (GUI) for ease of use.

## Features
### Sender
- GUI with a drop-down facility to select video files from the directory structure.
- Displays the status of the transfer in percentage.
- Shows a notification on successful file transfer.
- Opens the target folder after transfer completion.

### Receiver
- Opens a new file and writes received segments.
- Identifies the end of the file and terminates properly.

## Requirements
- GNU C Compiler
- GTK 3.0+
- Linux Operating System

## Instructions to Compile and Run
1. **Compile the Sender Code:**
   ```bash
   gcc sender.c -o sender `pkg-config --cflags --libs gtk+-3.0`
   ```
2. **Compile the Receiver Code:**
   ```bash
   gcc receiver.c -o receiver
   ```
3. **Run the Receiver Program First:**
   ```bash
   ./receiver
   ```
4. **Run the Sender Program:**
   ```bash
   ./sender
   ```

## File Structure
- `sender.c`: Sender program with GUI.
- `receiver.c`: Receiver program to save the received file.
- `README.txt`: Project overview and instructions.
- `Assignment_Document.docx`: Detailed design and description of the project.
