# NLW Spacetime | Backend

Memory recall application, where the user can add texts, photos and videos of important events in his life to a timeline, organized by month and year.

</br>

## 🔨 Features

- [x] Create account with Github
- [x] Login and logout with Github account
- [x] List of all users created memories
- [x] Create new memory
- [ ] Edit memory
- [ ] Delete memory
- [ ] Show specific memory

</br>

## 🧪 Tools

- [Node.js](https://nodejs.org/en)
- [TypeScript](https://www.typescriptlang.org/)
- [Fastify](https://www.fastify.io/)
- [Axios](https://axios-http.com/)
- [Prisma](https://www.prisma.io/)
- [zod](https://github.com/colinhacks/zod)

</br>

## 🧭 Getting Started

> _Before start, you need to have [Node.js](https://nodejs.org/en) installed on your machine and a code editor like [Visual Studio Code](https://code.visualstudio.com/)._

</br>

### Running the application:

- in terminal clone this project:

```bash
$ git clone https://github.com/palomarodrigs/spacetime-backend.git
```

- access the project folder:

```bash
$ cd spacetime-backend
```

- install dependencies:

```bash
$ npm install
```

- run server:

```bash
$ npm run dev

# If all goes well, this message will appear in the terminal:
🚀 HTTP server running on http://localhost:3333
```

</br>

### Creating an OAuth App:

- Go to the GitHub Developer Settings page: https://github.com/settings/developers.

- Click on "New OAuth App" to create a new OAuth App.

- Fill in the following information for your OAuth App:

  - Application Name: Choose a name for your application.
  - Homepage URL: http://localhost:3000. - change port if necessary.
  - Authorization callback URL: Enter the callback URL where GitHub will redirect users after authentication. For local development, we are using http://localhost:3000/api/auth/callback in the frontend.
  - Click on "Register Application" to create the OAuth App.

- After creating the OAuth App, you will see the `Client ID` and `Client Secret` on the OAuth App page. These credentials will be used to authenticate your application with GitHub.

- In your project, create a .env file in the root directory if it doesn't already exist.

- Set the DATABASE_URL environment variable

```bash
DATABASE_URL="file:./dev.db"
```

- Set the `GITHUB_CLIENT_ID` and `GITHUB_CLIENT_SECRET` environment variables, replacing `<CLIENT_ID>` and `<client_secret>` with your actual credentials obtained from the GitHub OAuth App page:

```bash
GITHUB_CLIENT_ID=<client_id>
GITHUB_CLIENT_SECRET=<client_secret>
```

> 💡 _Remember to keep your GitHub Client ID and Client Secret secure and never expose them publicly._

</br>

## 📝 License

This project is licensed under the MIT license. See the [LICENSE](https://github.com/palomarodrigs/spacetime-backend/blob/main/LICENSE) file for more details.

---

<p align="center">Developed with ❤️ by <a href="https://www.linkedin.com/in/paloma-rodrigues-539000233/" target="_blank">Paloma Rodrigues</a></p>
