# Introduction to Inter-Process Communication (IPC)

## 1. What is Inter-Process Communication (IPC)?

Inter-Process Communication (IPC) is a mechanism that allows two or more processes to communicate and exchange data with each other.

A process is a program that is currently running. Since processes usually have separate memory spaces, IPC provides methods for them to share information and coordinate their activities.

---

## 2. Definition and Meaning of IPC

**Inter-Process Communication (IPC)** refers to the techniques used by operating systems to allow processes to communicate, share data, and synchronize their activities.

In simple words:

> IPC allows different running programs or processes to talk to each other and exchange information.

Common IPC methods include:

- Pipes
- Message Queues
- Shared Memory
- Sockets
- Signals

---

## 3. Need for IPC

IPC is needed because processes often need to work together to complete a task.

The main purposes of IPC are:

- To exchange data between processes.
- To allow processes to work together.
- To share information and resources.
- To synchronize processes.
- To improve communication between different programs.
- To support client-server applications.

---

## 4. Why Do Processes Communicate?

Processes communicate for several reasons:

1. **Data Sharing** – One process may need data produced by another process.
2. **Resource Sharing** – Processes may need to share resources such as files or devices.
3. **Synchronization** – Processes may need to coordinate the order in which tasks are performed.
4. **Task Coordination** – A large task can be divided between multiple processes.
5. **Client-Server Communication** – A client process can request a service from a server process.

---

## 5. How Do Processes Communicate?

Processes can communicate using different IPC mechanisms.

### Common IPC Methods

| IPC Method | Description |
|---|---|
| Pipes | Used to send data from one process to another. |
| Message Queues | Processes communicate by sending and receiving messages. |
| Shared Memory | Multiple processes access a common area of memory. |
| Sockets | Used for communication between processes, including processes on different computers. |
| Signals | Used to notify a process that a particular event has occurred. |

---

## 6. Basic Client-Server Concept

The **client-server model** is a common example of process communication.

- **Client:** Requests a service or information.
- **Server:** Receives the request, processes it, and sends a response.

### Example

When you open a website:

1. Your browser acts as the **client**.
2. The browser sends a request to the web server.
3. The server processes the request.
4. The server sends the required webpage back to the browser.

```text
Client                         Server
  |                              |
  | ------ Request ------------> |
  |                              |
  | <------- Response ---------- |
  |                              |

<img width="233" height="148" alt="image" src="https://github.com/user-attachments/assets/26fe9213-07f6-4ff5-af60-f53dfc3e2b7d" />

