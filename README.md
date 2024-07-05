# Discord Clone

This project is a Discord clone built for my school Computer Science club. It offers real-time messaging, voice and video communication, and user authentication, among other features.

## Tech Stack

- **React**: A JavaScript library for building user interfaces.
- **Next.js 13**: A React framework for production.
- **Tailwind CSS**: A utility-first CSS framework.
- **Socket.io**: Enables real-time, bidirectional, and event-based communication.
- **Prisma**: Next-generation ORM for database management.
- **MongoDB**: A NoSQL database for storing application data.
- **Shadcn/ui**: A collection of modern UI components.
- **LiveKit**: For scalable WebRTC and real-time communication.
- **Uploadthing**: For handling file uploads.
- **Clerk**: Authentication and user management.

## Features

- **Real-time Messaging**: Instant communication using Socket.io.
- **Voice and Video Chat**: Powered by LiveKit for seamless communication.
- **User Authentication**: Managed by Clerk for secure login and registration.
- **Modern UI**: Styled with Tailwind CSS and Shadcn/ui components.
- **File Uploads**: Integrated with Uploadthing for handling file sharing.

## Setup

### Prerequisites

- Node.js
- npm or yarn
- MongoDB (local or cloud instance)
- Clerk account for authentication

### Installation

1. **Clone the repository**:
    ```sh
    git clone https://github.com/yourusername/discord-clone.git
    cd discord-clone
    ```

2. **Install dependencies**:
    ```sh
    npm install
    ```
    or
    ```sh
    yarn install
    ```

3. **Set up environment variables**:
    - Create a `.env` file in the project root and add the following variables:
        ```env
       NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=example
      CLERK_SECRET_KEY=example
      NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
      NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
      
      
      NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
      NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/
      
      
      DATABASE_URL="mongodb"
      
      UPLOADTHING_SECRET=example
      UPLOADTHING_APP_ID=example
      ```

4. **Run the Prisma migrations**:
    ```sh
    npx prisma migrate dev
    ```

### Running the Application

1. **Start the development server**:
    ```sh
    npm run dev
    ```
    or
    ```sh
    yarn dev
    ```

2. Open your browser and navigate to [http://localhost:3000](http://localhost:3000).

## Deployment

You can deploy your Next.js application on platforms like Vercel, Netlify, or any other cloud provider that supports Node.js.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request or open an issue to discuss what you would like to change.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Acknowledgements

- The developers and maintainers of all the libraries and frameworks used in this project.
- The members of my school CS club for their support and feedback.

