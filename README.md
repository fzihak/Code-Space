# Codespace 🚀

## About 📖

Codespace is a robust, open-source online judge platform designed for hosting competitive programming contests and coding challenges. Built with scalability and security in mind, it provides a comprehensive solution for educational institutions, coding bootcamps, and competitive programming enthusiasts.

## Features ✨

### For Users 👥
- **Seamless Authentication**
  - OAuth integration with GitHub and Google
  - Email verification and password recovery
  - Profile customization with coding statistics

- **Interactive Coding Environment** 💻
  - In-browser code editor with syntax highlighting
  - Support for 20+ programming languages
  - Code autocompletion and formatting
  - Custom input/output testing before submission

- **Learning Tools** 📚
  - Detailed problem explanations with examples
  - Editorial solutions after contest completion
  - Performance analytics and progress tracking
  - Practice mode with unlimited submissions

### For Contest Organizers 👨‍💼
- **Problem Management**
  - Rich text editor for problem descriptions
  - Custom test case generation
  - Multiple scoring criteria support
  - Automated difficulty assessment

- **Contest Administration** 🏆
  - Flexible contest scheduling
  - Custom scoring rules
  - Plagiarism detection
  - Real-time participant monitoring

### Technical Features 🛠️
- **Secure Execution Environment** 🔒
  - Isolated Docker containers for code execution
  - Resource limitation (CPU, memory, runtime)
  - Prevention of malicious code execution
  - Configurable security policies

- **Scalable Architecture** 📈
  - Microservices-based design
  - Redis-backed caching
  - RabbitMQ for asynchronous judging
  - Horizontal scaling support

## Tech Stack 🔧

- **Frontend**: React, TypeScript, TailwindCSS
- **Backend**: Node.js, Express, PostgreSQL
- **Execution**: Docker, Judge0
- **Infrastructure**: Redis, RabbitMQ, Nginx

## Installation 🚀

### Prerequisites
- Docker and Docker Compose
- Node.js ≥ 16
- PostgreSQL ≥ 13

### Quick Start ⚡
1. Clone the repository:
   ```bash
   git clone https://github.com/fzihak/codespace.git
   cd codespace
   ```

2. Configure environment variables:
   ```bash
   cp .env.example .env
   # Edit .env with your configuration
   ```

3. Start services using Docker Compose:
   ```bash
   docker-compose up -d
   ```

4. Initialize the database:
   ```bash
   npm run migrate
   npm run seed
   ```

5. Start development server:
   ```bash
   npm install
   npm run dev
   ```

Visit `http://localhost:3000` to access Codespace.

## Configuration ⚙️

### Database Setup
```env
DB_HOST=localhost
DB_PORT=5432
DB_NAME=codespace
DB_USER=postgres
DB_PASSWORD=your_password
```

### Judge Configuration
```env
JUDGE_MEMORY_LIMIT=512M
JUDGE_TIME_LIMIT=2s
JUDGE_OUTPUT_LIMIT=64K
```

## Contributing 🤝

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License 📝

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support 💬
- GitHub Issues: [Report bugs](https://github.com/fzihak/codespace/issues)
