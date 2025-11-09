# Invoice OCR to CSV

A Python tool that uses PaddleOCR to extract data from invoice images and convert them to CSV format.

## Features

- Processes multiple image formats (PNG, JPG, JPEG, TIFF, BMP)
- Extracts structured data from invoices
- Outputs data in CSV format with columns: Designation, Quantity, Unit Price, Amount
- Handles French number format
- Supports text orientation detection

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/invoice-ocr.git
cd invoice-ocr
```

2. Install the required packages:
```bash
pip install -r requirements.txt
```

## Usage

1. Place your invoice images in the project directory
2. Run the script:
```bash
python invoice_ocr.py
```
3. The processed CSV files will be saved in the `processed_invoices` directory

## Input Format

The script expects invoice images containing tables with the following columns:
- Designation (Product/Service description)
- Quantité (Quantity)
- Prix Unitaire (Unit Price)
- Montant (Amount)

## Output Format

The script generates CSV files with the following columns:
- Designation: Product or service description
- Quantité: Quantity
- Prix Unitaire: Unit price
- Montant: Total amount

## License

MIT License. See [LICENSE](LICENSE) file for details.