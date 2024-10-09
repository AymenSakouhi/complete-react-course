# React from 0 to Hero: 2-Day Professional Course

This course will guide you through the basics of Linux and the command line interface (CLI). Below are the key requirements to get started.

## Prerequisites for Linux + React:
1. **Basic Computer Skills**: Familiarity with basic operations like file management, navigating through an operating system, and using software applications.
2. **Access to a Linux Environment**: You will need access to a Linux system, which could be one of the following:
   - A physical Linux machine.
   - A Virtual Machine (VM) running Linux.
   - Windows Subsystem for Linux (WSL) on a Windows machine.
   - A cloud-based Linux environment (optional, but useful).

3. **Terminal/CLI Access**: You need to know how to open and operate a terminal. This could be:
   - A terminal emulator on Linux.
   - Bash, Zsh, or other shell environments on macOS.
   - WSL or PowerShell on Windows (with WSL installed).

4. **Text Editor**: You'll need a text editor to work with shell scripts or code. Some recommended options:
   - Terminal-based editors: Vim, Nano, Emacs.
   - Graphical editors: Visual Studio Code (with extensions for Linux and shell), Sublime Text, or Atom.

5. **No Prior Linux Experience Required**: This course is designed for beginners, so no prior knowledge of Linux or CLI is necessary, but enthusiasm and a willingness to learn are highly encouraged.

6. ** NVM (Node Version Manager) or NPM (Node Package Manager) **: You will need these tools to manage Node.js versions.

7. **Git**: You will need these tools to version control your code.


---

## Recommended Setup:
- **VSCode (Visual Studio Code)**: If you're using VSCode, consider installing the following extensions for a smoother workflow:
   - Remote - WSL (for WSL users).
   - ShellCheck (for shell scripting).
   - Markdown Preview Enhanced (if working with `.md` files).

---

By ensuring you have these tools and resources, you’ll be well-equipped to navigate through the course and become comfortable using Linux and the command line.

---

For more details and lessons, visit the [GitHub Repository](https://github.com/AymenSakouhi/complete-intro-to-linux-and-the-cli).


## Day 1: React Fundamentals (8 hours)

### Session 1: Introduction to React and Setting Up the Environment (1 hour)
**Goal**: Understand React basics and set up the development environment.
**Content**:
1. What is React? Why React for modern development?
2. React vs. other front-end frameworks (Angular, Vue).
3. How React works: Virtual DOM, JSX, Component-based architecture.
4. Setting up development tools:
   - Node.js, npm (or yarn)
   - Installing `create-react-app` (CRA)
5. Setting up Visual Studio Code (VSCode) with React extensions (Prettier, ESLint).
6. Running your first React app.

**Example**: Create a basic React app using `create-react-app`. Show how to start the server and examine the project structure.

---

### Session 2: React Components and JSX (2 hours)
**Goal**: Learn about JSX, functional components, and component props.
**Content**:
1. What is JSX? The syntax and advantages of JSX.
2. Creating functional components.
3. Passing props to components.
4. Rendering components in the App component.
5. Component composition (nesting components).

**Examples**:
- Create a `UserProfile` component that takes in `name`, `age`, and `role` props.
- Create a `UserList` component to display a list of user profiles.

---

### Session 3: State and Events (2 hours)
**Goal**: Learn how to manage component state and handle user events.
**Content**:
1. Introduction to React hooks (`useState`).
2. Using state to store and update data.
3. Handling events in React (e.g., button clicks, input changes).
4. Controlled vs. uncontrolled components (forms).

**Examples**:
- Build a `Counter` component with a button to increment and decrement a value using `useState`.
- Create a basic form where users can type in their name and role, and display it below using state.

---

### Session 4: React Lifecycle and `useEffect` (2 hours)
**Goal**: Understand the component lifecycle and how to use `useEffect`.
**Content**:
1. The lifecycle of a React component (Mounting, Updating, Unmounting).
2. Introduction to `useEffect` for side effects.
3. Fetching data from APIs with `useEffect`.
4. Cleaning up side effects in `useEffect`.

**Examples**:
- Fetch user data from a public API (e.g., JSONPlaceholder) and display it in a list.
- Implement a cleanup function in `useEffect` to demonstrate unmounting behavior.

---

### Session 5: Conditional Rendering and Lists (1 hour)
**Goal**: Learn how to conditionally render components and render lists of data.
**Content**:
1. Conditional rendering using ternary operators.
2. Rendering lists with `map()`.
3. Key prop importance in lists.

**Examples**:
- Display a message if the user list is empty.
- Render a list of users conditionally based on state.

---

### Homework/Project for Day 1:
Students will build a **basic Todo App**:
- Add, remove, and mark tasks as completed.
- Store tasks in state.
- Use conditional rendering to filter completed tasks.

---

## Day 2: Advanced React & University Forum App (8 hours)

### Session 1: React Router (1.5 hours)
**Goal**: Learn how to navigate between different pages in a React app.
**Content**:
1. Introduction to `react-router-dom`.
2. Setting up routes and navigating between pages.
3. Using `useParams` and `useHistory` for dynamic routes.

**Examples**:
- Create a simple app with Home, About, and Contact pages.
- Add navigation links between the pages.

---

### Session 2: React Context API and State Management (2 hours)
**Goal**: Understand how to manage global state using Context API.
**Content**:
1. Introduction to lifting state up and prop drilling issues.
2. Using React Context API to manage global state.
3. Creating a context provider and consumer.

**Examples**:
- Create a theme toggler with light and dark modes, using Context API to manage theme state globally.
- Implement user authentication state (logged in/out) across different pages.

---

### Session 3: Working with APIs using Axios & Fetch (2 hours)
**Goal**: Fetch and post data to external APIs.
**Content**:
1. Introduction to Axios and Fetch for HTTP requests.
2. Handling asynchronous requests.
3. Posting data to an API (e.g., creating a new user).

**Examples**:
- Fetch forum posts from an API and display them.
- Post new forum posts from a form submission using Axios.

---

### Session 4: Building the University Forum App (2.5 hours)
**Goal**: Build and deploy a complete University Forum App by integrating all concepts.

**App Requirements**:
1. A home page showing all forum posts.
2. A page for creating a new post.
3. A post details page.
4. User login/logout functionality (mock with Context API).
5. Fetch forum data from a JSON file or API.

**Step-by-Step Guide**:
1. Setting up the Project: Create a new React app using `create-react-app` with basic routing and folder structure.
2. Components:
   - Navbar: Home, Login, Create Post.
   - PostList: Display all posts.
   - PostDetail: View individual post details.
   - NewPost: Form to create a new post.
   - LoginPage: Mock login using Context API.
3. State and Context Management:
   - Create a `UserContext` to manage authentication state.
   - Use `useState` and `useEffect` to manage post data (mock data).
4. API Integration:
   - Use Axios to fetch posts from a mock API.
   - Implement POST request for new posts.
5. Routing:
   - Use `react-router-dom` to set up routes for home, post details, and new post pages.

---

### Session 5: Deploying with PM2 (1 hour)
**Goal**: Deploy the University Forum App on a server with PM2.
**Content**:
1. Build the React app using `npm run build`.
2. Introduction to PM2 and Node.js as a production server.
3. Setting up a simple Express server to serve the React app.
4. Installing PM2 and running the Express server with PM2.
5. Monitoring and restarting the app with PM2.

**Example**:
- Set up a basic Express server.
- Deploy the built React app using PM2 for process management.

---

### Final Project:
The **University Forum App** will be fully functional, deployed, and monitored with PM2. It will include:
- User authentication (mocked).
- API integration.
- A forum to create and display posts.

---

### Additional Notes:
- **Resources**: Provide students with links to React documentation, useful articles, and videos for further learning.
- **Assessment**: At the end of the course, assess the students based on the completion of the final project and a few conceptual questions on React basics.
