# Automated Fake Social Media Account Detection Tool

## Overview
The **Automated Fake Social Media Account Detection Tool** is a comprehensive solution that identifies and flags fake profiles across platforms such as Instagram, Facebook, Twitter, and LinkedIn. Combining a machine learning backend with an intuitive frontend interface, this project provides users with a seamless way to analyze and report suspicious accounts.

---

## Frontend

### Features
- **Machine Learning Integration**: Interacts with backend APIs to leverage trained ML models for detecting fake accounts.
- **User-Friendly Interface**: Built with React.js, the frontend offers a clean and intuitive user experience.
- **Scalable Architecture**: Optimized for performance and scalability, ensuring smooth operation even with high traffic.
- **Navigation and Dashboard**: Provides quick access to tools like account verification, reporting, and an admin panel.
  - **Dashboard Statistics**:
    - Accounts Verified
    - Fake Accounts Detected
    - Reports Processed
    - Success Rate

### Installation and Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/pnnv/fotodile
   cd fotodile
   ```
2. Install dependencies:
   ```bash
   npm install
   npm install lucide-react@0.263.1
   ```
3. Start the development server:
   ```bash
   npm run dev -- --open
   ```

---

## Backend

### Features
#### Machine Learning Algorithms
- Utilizes classification models like Random Forest, AdaBoost, Decision Tree, Logistic Regression, and SVM for high-accuracy predictions.
- Processes account data to classify profiles as real or fake.

#### Feature Engineering
- Scrapes and analyzes key account features:
  - **Profile Picture**: Checks for presence or absence.
  - **Username Patterns**: Examines length, format, and keywords.
  - **Follower-to-Following Ratio**: Compares numerical metrics.
  - **Account Activity**: Measures post frequency and engagement levels.
  - **Verification Status**: Identifies whether the account is verified.

#### Centralized Reporting System
- Flags detected fake accounts and coordinates actions like suspension or deletion with social media platforms.

#### API Integration
- Built with Flask and FastAPI to handle data processing and predictions.
- Deployed on platforms like Heroku or AWS for scalability.

### Workflow
1. **Input Form**: Users submit social media account links for analysis.
2. **Data Scraping**: Extracts account features using Python-based HTML parsing.
3. **Feature Vector Generation**: Converts extracted data into structured inputs for ML models.
4. **ML Classification**: Predicts the likelihood of an account being fake.
5. **Results Visualization**: Outputs results in a tabular format with interactive visualizations.
6. **Reporting**: Sends flagged accounts to a central agency for further action.

### Technical Architecture
- **Frontend**: React.js
- **Backend**: Flask and FastAPI
- **Machine Learning**: Algorithms include Random Forest, AdaBoost, Logistic Regression, Decision Tree, KNN, and SVM.
- **Deployment**: Hosted on Heroku or AWS, with GitHub for version control.

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/pnnv/fotodile
   cd fotodile
   ```
2. Install dependencies:
   ```bash
   cd backend
   pip install -r requirements.txt
   ```
3. Run the application:
   ```bash
   python app.py
   ```

---

## Contribution
Contributions are welcome! Follow these steps:
1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature-branch-name
   ```
3. Commit your changes and push the branch:
   ```bash
   git push origin feature-branch-name
   ```
4. Open a pull request.

---

## License
This project is licensed under the MIT License. See the LICENSE file for details.

---

## Contact
For queries or support, reach out through the [Issues](https://github.com/fotodile/issues) section.

