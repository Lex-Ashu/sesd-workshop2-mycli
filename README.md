# MyCLI - SESD Workshop 2 Project

A CLI tool built with Node.js, TypeScript, and Object-Oriented Programming principles.

## Setup Instructions

1. Clone the repository:
```bash
git clone <your-repo-url>
cd cli-workshop
```

2. Install dependencies:
```bash
npm install
```

3. Build the project:
```bash
npm run build
```

4. Test the CLI:
```bash
node dist/cli.js --help
```

## Available Commands

### 1. Greet Command
```bash
mycli greet <name>
```
Example: `mycli greet John` → Output: Hello John!

### 2. Math Commands
```bash
mycli add <num1> <num2>
mycli sub <num1> <num2>
mycli mul <num1> <num2>
mycli div <num1> <num2>
```
Example: `mycli add 5 3` → Output: 5 + 3 = 8

### 3. Joke Command (API)
```bash
mycli joke
```
Fetches a random joke from Official Joke API

### 4. GitHub Command (API)
```bash
mycli github <username>
```
Example: `mycli github torvalds` → Shows GitHub user info

### 5. Quote Command (API)
```bash
mycli quote
```
Fetches a random inspirational quote

### 6. Dog Command (API)
```bash
mycli dog
```
Fetches a random dog image URL

### 7. Advice Command (API)
```bash
mycli advice
```
Fetches random advice

### 8. File Info Command
```bash
mycli fileinfo <filename>
```
Example: `mycli fileinfo package.json` → Shows file details

### 9. Help Command
```bash
mycli --help
```

### 10. Version Command
```bash
mycli --version
```

## Example Usage
```bash
# Build the project
npm run build

# Run commands
node dist/cli.js greet Alice
node dist/cli.js add 10 20
node dist/cli.js joke
node dist/cli.js github octocat
node dist/cli.js quote
```

## Project Structure
```
cli-workshop/
├── cli.ts                 # Main entry point
├── commands/              # Command classes
│   ├── GreetCommand.ts
│   ├── MathCommand.ts
│   ├── JokeCommand.ts
│   ├── GithubCommand.ts
│   ├── QuoteCommand.ts
│   ├── DogCommand.ts
│   ├── AdviceCommand.ts
│   └── FileInfoCommand.ts
├── interfaces/
│   └── ICommand.ts
├── package.json
├── tsconfig.json
└── README.md
```

## APIs Used

1. **Official Joke API** - https://official-joke-api.appspot.com/
2. **GitHub API** - https://api.github.com/
3. **Quotable API** - https://api.quotable.io/
4. **Dog CEO API** - https://dog.ceo/api/
5. **Advice Slip API** - https://api.adviceslip.com/

## OOP Concepts

- **Classes**: Each command is a separate class
- **Interfaces**: ICommand interface for all commands
- **Encapsulation**: Command logic in respective classes
- **Object Creation**: Command instances in main CLI

## Technologies

- Node.js
- TypeScript
- Commander.js
- Axios

## Author
Ashu Choudhary
