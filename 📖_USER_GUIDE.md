# 🚀 Bill Generator V04 - User Guide

## 🎯 What is Bill Generator V04?

Bill Generator V04 is a professional Streamlit application that generates A4 documents including:
- **Deviation Statements** (Landscape format)
- **Work Orders**
- **Scrutiny Sheets**
- **Acceptance Letters**
- **Comparative Statements**

## 🚀 Quick Start (3 Easy Steps)

### Option 1: One-Click Launch (Recommended for Beginners)
1. **Double-click** `🚀_LAUNCH_APP.bat`
2. **Wait** for the app to load in your browser
3. **Upload** your Excel file and start generating documents!

### Option 2: Full Setup (For Advanced Users)
1. **Double-click** `zzz_run_app.bat` (installs dependencies first time)
2. **Wait** for installation to complete
3. **App opens automatically** in your browser

## 📁 Required Files

### Excel File Format
Your Excel file should contain these columns:
- **Serial No.** - Item number
- **Description** - Item description
- **Unit** - Unit of measurement
- **Quantity** - Amount needed
- **Rate** - Price per unit
- **Amount** - Total cost

### Supported Formats
- `.xlsx` (Excel 2007+)
- `.xls` (Excel 97-2003)

## 🎨 Features

### ✅ **Deviation Statement** - **LANDSCAPE FORMAT**
- Automatically prints in landscape orientation
- Professional A4 layout with 10mm margins
- Calculates excess/savings automatically

### ✅ **Multiple Output Formats**
- **HTML** - View in browser
- **PDF** - Professional printing
- **DOCX** - Microsoft Word editing

### ✅ **Smart Calculations**
- Automatic total calculations
- Number to words conversion
- Professional formatting

## 🔧 Troubleshooting

### ❌ **App won't start?**
1. Make sure Python is installed
2. Run `zzz_run_app.bat` to install dependencies
3. Check if port 8501 is free

### ❌ **Documents not generating?**
1. Check Excel file format
2. Ensure all required columns are present
3. Verify file isn't corrupted

### ❌ **PDF not working?**
1. The app automatically downloads wkhtmltopdf if needed
2. Check internet connection for first-time setup

## 🌐 Deployment Options

### **Streamlit Cloud (Recommended)**
1. Push code to GitHub
2. Connect to Streamlit Cloud
3. Deploy automatically

### **Local Network**
1. Run the app locally
2. Share your IP address with team members
3. They can access via `http://YOUR_IP:8501`

## 📞 Support

- **For Issues**: Check the troubleshooting section above
- **For Features**: The app automatically handles most common scenarios
- **For Deployment**: Use the provided .bat files

## 🎉 Pro Tips

1. **Use the one-click launcher** (`🚀_LAUNCH_APP.bat`) for daily use
2. **Keep Excel files organized** for faster processing
3. **The app remembers your settings** between sessions
4. **All documents are A4 format** with professional margins

---

**Happy Bill Generating! 🎯📄**
