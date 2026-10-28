# Computer Networks (CN) Laboratory Programs

This repository contains C implementations of fundamental Computer Networks and Data Communication concepts, protocols, and algorithms.

---

## 📁 Repository Structure

| Folder | Topic / Protocol | Files | Description |
| :--- | :--- | :--- | :--- |
| **`bitStuff/`** | Bit Stuffing | `transmitter.c`, `receiver.c` | Framing using bit stuffing (inserting 0 after five consecutive 1s) and de-stuffing |
| **`byteCount/`** | Character / Byte Count | `transmitter.c`, `receiver.c` | Framing using character/byte count method |
| **`byteStuff/`** | Byte Stuffing | `transmitter.c`, `receiver.c` | Framing using byte stuffing (character stuffing with escape sequences) |
| **`Calculator/`** | Socket Calculator | `Calculator_Server.c`, `Calculator_Client.c` | TCP client-server arithmetic calculator over socket communication |
| **`CRC/`** | Cyclic Redundancy Check | `transmitter.c`, `receiver.c` | Error detection using CRC polynomial division |
| **`DSSS/`** | Direct Sequence Spread Spectrum | `DSSS_Transmitter.c`, `DSSS_Receiver.c` | DSSS modulation and demodulation simulation using PN sequence / chipping code |
| **`FHSS/`** | Frequency Hopping Spread Spectrum | `freqHop_Transmitter.c`, `freqHop_Receiver.c` | FHSS simulation with pseudo-random frequency hopping pattern |
| **`GBN/`** | Go-Back-N ARQ Protocol | `transmitter.c`, `transmitter2.c`, `receiver.c` | Sliding window flow and error control using Go-Back-N mechanism |
| **`Hamming/`** | Hamming Code | `transmitter.c`, `receiver.c` | Error detection and correction using Hamming (7,4) code |
| **`slidWin/`** | Sliding Window Protocol | `transmitter.c`, `receiver.c` | General sliding window flow control protocol implementation |
| **`SR/`** | Selective Repeat ARQ Protocol | `transmitter.c`, `receiver.c` | Selective Repeat protocol for retransmitting only corrupted/lost frames |
| **`swNoiceless/`** | Stop-and-Wait (Noiseless) | `transmitter.c`, `receiver.c` | Elementary Stop-and-Wait protocol over an error-free channel |
| **`swNoisy/`** | Stop-and-Wait (Noisy) | `transmitter.c`, `receiver.c` | Stop-and-Wait ARQ protocol with ACK, NAK, and timeout for noisy channels |
| **`UDP/`** | UDP Client-Server | `serverUDP.c`, `clientUDP.c` | Connectionless socket communication using User Datagram Protocol |

---

## 🛠️ Compilation and Execution

### Prerequisites
- GCC compiler (`gcc`)
- Linux / POSIX environment (e.g., Ubuntu, WSL, macOS) or MinGW on Windows

### Example: Running a Client-Server or Transmitter-Receiver Pair

1. **Open two terminal windows** (Terminal 1 for Receiver / Server, Terminal 2 for Transmitter / Client).

2. **Compile the programs**:
   ```bash
   # Receiver / Server
   gcc -o receiver receiver.c

   # Transmitter / Client
   gcc -o transmitter transmitter.c
   ```

3. **Run the Receiver / Server first**:
   ```bash
   ./receiver
   ```

4. **Run the Transmitter / Client**:
   ```bash
   ./transmitter
   ```
