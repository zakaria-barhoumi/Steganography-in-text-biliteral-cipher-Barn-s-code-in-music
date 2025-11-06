# Steganography in Text (Biliteral Cipher, Barn's Code) & in Music

**Authors:** Zakaria Barhoumi and Aziz Ayari

---

## 1. Abstract

This project investigates **steganography**: the practice of concealing the existence of a secret message within an apparently innocuous medium (the "cover").

We explore and demonstrate three distinct techniques across two media:
* **Text:** Using the Biliteral (Bacon's) Cipher and Barn's Code.
* **Music:** Using both symbolic (notation) and digital (audio file) methods.

## 2. Textual Steganography Methods

### 2.1. Biliteral Cipher (Bacon's Cipher)
A method that encodes each letter of a secret message into a 5-bit binary sequence (e.g., `A = aaaaa`, `B = aaaab`). These binary digits (`a`/`b`) are then represented by subtle typographic variations (e.g., *italic* vs. regular font) in a cover text.

### 2.2. Barn's Code
A grille-based steganographic method where a shared secret keyword determines the order for selecting specific words from a cover text. When extracted in the correct sequence, these words form the hidden message.

## 3. Musical Steganography Methods

### 3.1. Symbolic (Notation-Based)
This approach embeds data within the musical score itself.
* **Note-Mapping:** Assigning notes to letters (e.g., C = 'A', D = 'B').
* **Rhythmic Encoding:** Using note durations to represent binary data (e.g., quarter note = `0`, eighth note = `1`).

### 3.2. Digital (Audio LSB)
This technique modifies the **Least Significant Bit (LSB)** of each sample in a digital audio file (e.g., `.WAV`). This alteration is imperceptible to the human ear but allows for a large volume of data to be embedded directly into the audio stream.

## 4. Repository Contents

* `/presentation/`: Project slides and research notes.
* `/examples/`: Demonstration files for each technique (text and audio).
* `/src/`: Encoder/decoder scripts.
