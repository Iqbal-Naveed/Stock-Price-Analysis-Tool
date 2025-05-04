# Stock-Price-Analysis-Tool
Stock Price Analysis Tool (C++)
Overview
This is a Stock Price Analysis Tool built using C++ and the raylib library. The tool allows users to select a company, visualize its stock price data over time, and analyze the best days to buy and sell for the maximum profit. It supports multiple companies, and users can interactively navigate through the data, viewing charts and analysis results.

Features
Company Selection: Choose from a list of companies (Meezan Bank, HBL, Bank Al Habib Ltd, UBL).

Interactive Stock Price Visualization: Display stock prices over time in a line graph.

Profit Analysis: Automatically calculates and highlights the best buy and sell days for maximum profit.

Customizable: The stock data is loaded from text files for each company, and the tool adapts to any data provided in the correct format.

Back Navigation: Users can go back to the company selection screen to choose another company.

Prerequisites
To compile and run this tool, you will need:

A C++ compiler (e.g., g++ or Clang).

The raylib library. raylib installation guide.

Standard C++ library (no external libraries other than raylib are required).

A terminal that supports raylib and graphics rendering (on Windows, Linux, or macOS).

Files
stock_analysis.cpp: The C++ source code for the stock price analysis tool.

MeezanBank.txt, HBL.txt, BankAlHabib.txt, UBL.txt: Stock price data files for each company. These files should be placed in the same directory as stock_analysis.cpp.

Makefile (optional): A build script for easy compilation.

Compilation
Install raylib by following the raylib installation guide.

Open your terminal and navigate to the directory containing stock_analysis.cpp.

Compile the program using the following command (ensure you link raylib during compilation):

bash
g++ -o stock_analysis stock_analysis.cpp -lraylib -lm -lpthread -ldl -lrt -lX11
Run the program:

bash
./stock_analysis
Stock Data Format
Each stock data file (e.g., MeezanBank.txt) should contain lines with the following format:

css
YYYY-MM-DD <price>
Where:

YYYY-MM-DD is the date of the stock price.

<price> is the stock price on that date.

For example:

yaml
2023-01-01 150
2023-01-02 152
2023-01-03 148
The program expects this format to load the stock prices correctly.

Game Instructions
Upon starting the program, you will see a list of companies.

Use the UP and DOWN arrow keys to navigate through the list of companies.

Press ENTER to select a company. The stock data for that company will be loaded and displayed.

The program will automatically calculate the best buy and sell days to maximize profit.

Green lines represent the optimal buy-sell period for maximum profit.

You can see the detailed analysis (buy/sell dates, prices, and maximum profit) displayed at the top.

Press BACKSPACE to return to the company selection screen and choose another company.

Game Controls
UP / DOWN Arrow: Navigate between the companies.

ENTER: Select a company.

BACKSPACE: Go back to the company selection screen.

Example Gameplay
markdown
Select a Company:
1. Meezan Bank
2. HBL
3. Bank Al Habib Ltd
4. UBL

Press ENTER to select a company.
After selecting a company, the stock chart will be displayed, and the best buy and sell days will be highlighted.

Visual Representation
The application uses raylib to display:

A line graph representing stock prices over time.

A green line indicating the optimal buy-sell period for maximum profit.

Axis labels for price and days.

Troubleshooting
Problem: The stock price chart is not displaying.

Solution: Ensure that raylib is installed correctly and your terminal/IDE supports graphics rendering.

Problem: The data file is not being loaded.

Solution: Ensure the stock data file is in the correct format (one line per date and price) and located in the same directory as the program.

License
This tool is free to use and modify. You are welcome to enhance or extend it for your needs.

Author 
Naveed Iqbal
CT-22051
