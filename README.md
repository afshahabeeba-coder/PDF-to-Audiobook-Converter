# PDF-to-Audiobook Converter

A powerful tool that converts PDF documents into high-quality audiobooks using advanced text-to-speech technology.

## Features

- **PDF Processing**: Extracts text from PDF files accurately
- **Text-to-Speech**: Converts extracted text to natural-sounding audio
- **Multiple Voices**: Support for various voice options and languages
- **Audio Format Support**: Generate audiobooks in MP3, WAV, and other formats
- **Batch Processing**: Convert multiple PDFs in one operation
- **Customization**: Adjust speed, pitch, and voice settings
- **Progress Tracking**: Real-time conversion status updates

## Requirements

- Python 3.8 or higher
- pip package manager

## Installation

```bash
git clone https://github.com/afshahabeeba-coder/PDF-to-Audiobook-Converter.git
cd PDF-to-Audiobook-Converter
pip install -r requirements.txt
```

## Usage

```bash
python converter.py --input sample.pdf --output sample_audiobook.mp3
```

### Command Line Options

- `--input`: Path to the PDF file to convert
- `--output`: Output audio file path
- `--voice`: Voice option (default: 'en-US')
- `--speed`: Speech speed (0.5 - 2.0, default: 1.0)
- `--format`: Output format (mp3, wav, default: 'mp3')

## Configuration

Edit `config.json` to customize default settings:

```json
{
  "default_voice": "en-US",
  "default_speed": 1.0,
  "default_format": "mp3",
  "max_file_size_mb": 100
}
```

## Supported Languages

- English (US, UK, AU, IN)
- Spanish
- French
- German
- Italian
- Portuguese
- Japanese
- Mandarin Chinese
- And more...

## API Reference

### PDFConverter Class

```python
from converter import PDFConverter

converter = PDFConverter()
converter.convert('input.pdf', 'output.mp3', voice='en-US', speed=1.0)
```

## Error Handling

The converter includes robust error handling for:
- Invalid PDF files
- Corrupted documents
- Unsupported formats
- File I/O errors

## Performance

Typical conversion times:
- 100-page PDF: ~5-10 minutes
- 500-page PDF: ~25-50 minutes
- Performance varies based on system resources and voice selection

## Troubleshooting

**Issue**: PDF won't open
- **Solution**: Ensure the PDF is not corrupted and is in standard format

**Issue**: Audio quality is poor
- **Solution**: Check your voice selection and try a different language/voice option

**Issue**: Conversion is slow
- **Solution**: Close other applications and free up system resources

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Support

For issues, questions, or suggestions, please open an issue on the [GitHub Issues](https://github.com/afshahabeeba-coder/PDF-to-Audiobook-Converter/issues) page.

## Authors

- **Afsha Habeeba** - Initial work - [GitHub](https://github.com/afshahabeeba-coder)

## Acknowledgments

- Text extraction powered by PyPDF2
- Text-to-speech powered by gTTS and pyttsx3
- Audio processing using ffmpeg

## Changelog

### Version 1.0.0 (2024)
- Initial release
- Basic PDF to audio conversion
- Multi-language support
- Batch processing capability
