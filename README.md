<div align="center">
  <h1>Node Multi-Threading </h1>
  <img src="https://c.tenor.com/i1mtd-XCEj8AAAAC/tenor.gif" width="300" alt="Multi-threading" />
    <img src="https://c.tenor.com/i1mtd-XCEj8AAAAC/tenor.gif" width="300" alt="Multi-threading" />
      <img src="https://c.tenor.com/i1mtd-XCEj8AAAAC/tenor.gif" width="300" alt="Multi-threading" />
  
  **A simple demonstration of using Worker Threads in Node.js for parallel image processing**

  [![Node.js](https://img.shields.io/badge/Node.js-18+-339933?style=for-the-badge&logo=node.js)](https://nodejs.org/)
  [![Jimp](https://img.shields.io/badge/Jimp-Image%20Processing-orange?style=for-the-badge)](https://github.com/jimp-dev/jimp)
</div>

---

## About

This project shows how to use **Node.js Worker Threads** to process images in parallel (resizing + compression) without blocking the main thread.

It compares:
- **Single-threaded** processing (`normal.js`)
- **Multi-threaded** processing using `worker_threads` (`multithreading.js`)

Great for learning how to speed up CPU-intensive tasks like image manipulation in Node.js.

## Performance Results

==============================
NORMAL PROCESSING
==============================
Total time: 7622ms (7.62s)
Average image time: (762ms)
==============================

==============================
MULTI THREADING PROCESSING
==============================
Total time: 2677ms (2.68s)
Average image time: (268ms)
==============================

## Features

- Parallel image processing with Worker Threads
- Uses **Jimp** for resizing and compressing images
- Non-blocking main thread
- Side-by-side comparison with normal (sequential) processing
- Clean folder structure for input and output images


## How to Run

1. Clone the repo
   git clone https://github.com/konhito/Node-Multi-Threading.git
   cd Node-Multi-Threading

2. Install dependencies
   npm install

3. Add some images to the input-images/ folder

4. Run single-threaded version:
   node normal.js

5. Run multi-threaded version:
   node multithreading.js

6. Check results.txt for performance comparison and look at the output folders.

## Why Use Worker Threads?

Node.js is single-threaded by default. Worker Threads allow you to run JavaScript in parallel, which is very useful for heavy tasks like image processing.

Made for learning Node.js performance.
