from PyPDF2 import PdfMerger

merger = PdfMerger()

pdf_files = ["file1.pdf", "file2.pdf", "file3.pdf"]

for pdf in pdf_files:
    merger.append(pdf)

merger.write("merged_output.pdf")
merger.close()

print("✅ PDFs merged successfully into 'merged_output.pdf'")
