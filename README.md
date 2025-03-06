# rustwc

A Rust implementation of the BSD wc (word count) program, designed to provide accurate word, line, character, and byte counting functionality similar to the classic BSD wc utility.

## About

`rustwc` is a modern, efficient implementation of the word count utility written in Rust. It provides accurate counting of:
- Lines (-l, --lines)
- Words (-w, --words)
- Characters (-m, --chars)
- Bytes (-c, --bytes)

Key features:
- Unicode support using the unicode-segmentation crate for accurate word boundaries
- Efficient streaming processing of files
- Support for multiple input files
- Standard input support when no files are specified

## Credits

This program was developed by Cline with assistance from Claude, an AI model by Anthropic. The implementation follows the BSD wc utility's functionality while leveraging Rust's safety and performance features.

## Installation

You can install rustwc using the provided RPM or DEB packages from the latest GitHub release.

### DEB package (Debian/Ubuntu):
```bash
sudo dpkg -i rustwc_*.deb
```

### RPM package (Fedora/RHEL):
```bash
sudo rpm -i rustwc-*.rpm
```

## Usage

```bash
rustwc [OPTIONS] [FILE]...

Options:
  -c, --bytes     Print the byte counts
  -m, --chars     Print the character counts
  -l, --lines     Print the newline counts
  -w, --words     Print the word counts
  -h, --help      Print help
  -V, --version   Print version
```

## License

This project is licensed under the MIT License
