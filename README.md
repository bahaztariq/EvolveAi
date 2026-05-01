# EvolveAi (Income AI MVC)

EvolveAi is a custom PHP MVC web application designed to help users identify their goals, build their skills, and discover new income opportunities. Leveraging the power of AI (via Google Gemini), the platform provides personalized learning plans, daily tasks, and actionable feedback to guide users toward their career and financial objectives.

## 🚀 Features

- **Personalized Skill Tracking:** Track current skills, mastery levels, and areas of interest.
- **AI-Powered Learning Plans:** Automatically generate AI plans with targeted goals and daily tasks based on user surveys and chosen opportunities.
- **AI Feedback:** Receive automated feedback on submitted tasks to ensure continuous improvement.
- **Opportunity Discovery:** Explore new career paths and income opportunities tailored to your skill set.
- **Community Engagement:** Read, write, and interact with community articles. Share your journey and learn from others.
- **User Authentication:** Secure signup, login, and password reset functionalities.

## 🛠️ Tech Stack

- **Backend:** Custom PHP MVC Architecture
- **Database:** PostgreSQL
- **AI Integration:** Google Gemini PHP Client
- **Environment Management:** vlucas/phpdotenv
- **HTTP Client:** Symfony HTTP Client & PSR-7
- **Mailing:** PHPMailer

## 📂 Project Structure

```text
├── app/                  # Application core
│   ├── Controllers/      # Handles incoming requests and logic
│   ├── Core/             # Base MVC classes (Router, Controller, etc.)
│   ├── Middlewares/      # Request filters (e.g., Auth)
│   ├── Models/           # Database interaction and entities
│   ├── Repositories/     # Data access layer
│   ├── Services/         # Business logic and AI integrations
│   └── Views/            # Frontend templates
├── config/               # Configuration files (DB, Mail, App settings)
├── database/             # Database schemas and seed scripts
├── docs/                 # Project documentation and UML
├── public/               # Web root (index.php, CSS, JS, images)
└── vendor/               # Composer dependencies
```

## 🏁 Getting Started

### Prerequisites

- PHP 8.1 or higher
- PostgreSQL
- Composer

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/bahaztariq/EvolveAi.git
   cd EvolveAi
   ```

2. **Install dependencies:**
   ```bash
   composer install
   ```

3. **Environment Configuration:**
   Copy the `.env.example` file to `.env` and fill in your credentials.
   ```bash
   cp .env.example .env
   ```
   *Make sure to provide your database credentials, Mailer config, and Google Gemini API Key.*

4. **Database Setup:**
   Create a PostgreSQL database named `evolve_ai` and run the schema file located at `database/database.sql` to generate the necessary tables.

5. **Run the Application:**
   Start the built-in PHP development server from the `public` directory:
   ```bash
   cd public
   php -S localhost:8000
   ```
   Visit `http://localhost:8000` in your browser.

## 🤝 Contributing

Contributions are welcome! Feel free to submit a Pull Request.

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
