# Gold Micro Optimizer

A decision tool for optimizing micro gold purchases. Available as both a bash script and a web application.

## Features

- Calculates RM/g (cost per gram) for different micro gold sizes
- Identifies the best option with lowest RM/g
- Shows profit/loss calculations based on bank buy-back price
- Saves previous values for quick updates
- Available as:
  - **Bash script** for command-line use
  - **Web application** for browser use (deployable to GitHub Pages)

## Web Application

The web version (`index.html`) provides:
- Modern, responsive UI
- LocalStorage to remember previous values
- Real-time calculations
- Mobile-friendly design

### Deploying to GitHub Pages

1. **Create a GitHub repository** (if you haven't already):
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git remote add origin https://github.com/YOUR_USERNAME/gold-micro-optimizer.git
   git push -u origin main
   ```

2. **Enable GitHub Pages**:
   - Go to your repository on GitHub
   - Click on **Settings**
   - Scroll down to **Pages** section
   - Under **Source**, select **Deploy from a branch**
   - Choose **main** branch and **/ (root)** folder
   - Click **Save**

3. **Your site will be live at**:
   ```
   https://YOUR_USERNAME.github.io/gold-micro-optimizer/
   ```

## Bash Script Usage

1. Make the script executable:
   ```bash
   chmod +x gold_micro_optimizer
   ```

2. Run the script:
   ```bash
   ./gold_micro_optimizer
   ```

3. Enter the bank buy-back price and today's prices for each micro gold size.

4. The script will:
   - Show calculations for each size
   - Identify the best option (lowest RM/g)
   - Save your inputs for next time

## Inputs Required

- **Bank buy-back price**: Current buy-back rate per gram
- **Micro gold prices**:
  - 0.015g
  - 0.016g
  - 0.017g
  - 0.018g
  - 0.020g
  - 0.025g

## How It Works

The tool calculates:
- **RM/g**: Cost per gram (price ÷ grams)
- **Bank Value**: What the bank would pay (grams × buy-back price)
- **Profit/Loss**: Bank value minus purchase price

The **best recommendation** is the micro gold size with the **lowest RM/g**, which gives you the most gold for your money.

## License

Free to use for personal purposes.
