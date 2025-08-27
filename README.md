# PDF_merger_tool
# PDF Merger Tool
# This program merges multiple PDF files into one

from PyPDF2 import PdfMerger

# Create a PdfMerger object
merger = PdfMerger()

# List of PDF files to merge
pdf_files = ["file1.pdf", "file2.pdf", "file3.pdf"]  # Apne files ke naam yaha likho

# Add each PDF to the merger
for pdf in pdf_files:
    merger.append(pdf)

# Save the merged PDF
merger.write("merged_output.pdf")
merger.close()

print("✅ PDFs merged successfully into 'merged_output.pdf'")
