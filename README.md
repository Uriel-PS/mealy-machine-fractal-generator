# Mealy Machine Simulator

Project developed for the Formal Languages and Automata Theory course, Computer Science program at UDESC (Universidade do Estado de Santa Catarina).

Simulates a **Mealy Machine** that reads a formal automaton specification and an input word, producing a **PPM image (P1 format)** as output. Since a Mealy Machine's output depends on both the current state and the input symbol, feeding it different words generates different fractal-like patterns.

**Author:** Uriel Pacheco de Souza
**Instructor:** Karina Girardi Roggia
**Term:** 2025/2

## How It Works

1. Reads a `.txt` file describing the Mealy Machine (initial state, transitions, and outputs).
2. Reads a `.txt` file with the input word (symbols `{1,2,3,4,.,N}`).
3. Simulates the machine step by step, producing a sequence of `0`s, `1`s, and line breaks as output.
4. Converts that output into a **PPM (P1) image**, viewable directly (e.g. in Google Colab) or convertible to `.png`.

## Usage

```bash
python3 mealy.py <machine_spec.txt> <input_word.txt> <output.ppm>
```

Example:
```bash
python3 mealy.py "Maquinas de Mealy/m1.txt" "Palavras/w16.txt" output.ppm
```

## Repository Structure

```
mealy.py                 # Simulator
Maquinas de Mealy/        # Sample Mealy Machine specifications
Palavras/                 # Sample input words of varying length
Relatório LFA - URIEL.pdf # Full academic report (Portuguese)
```

## Documentation

The full report, including the formal definition of the automaton, design decisions, and example outputs, is available in this repository as a PDF (in Portuguese).
