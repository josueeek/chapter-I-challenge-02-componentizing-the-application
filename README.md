<h1 align="center">
  <img alt="ignite-reactjs" title="ignite-reactjs" src=".github/cover-reactjs.png">
</h1>

# 💻 About the challenge

In this challenge, you'll have to create an application to train what you've learned so far in ReactJS

This will be an application where your main objective is to refactor a movie listing page according to genre.

The application is now fully functional but most of its code is directly in the `App.tsx` file. To solve this in the best way, it is necessary to divide the application into **at least** two main parts: sidebar and the main content that has the header and the movie listing.

- The application has only one main feature which is the movie listing;
- In the sidebar it is possible to select which category of movies should be listed;
- The first category in the list (which is "Action") must already start as marked;
- The application header only has the name of the selected category, which should change dynamically.

Below we will see in more detail what and how it needs to be done 🚀

## Application Template

To help you with this challenge, we've created this template for you that you should use as a GitHub template.

The template is available in the following [URL](https://github.com/rocketseat-education/ignite-template-componentizando-a-aplicacao).

**Tip**: If you don't know how to use GitHub repositories as a template, we have a guide at **[our FAQ](https://www.notion.so/FAQ-Desafios-ddd8fcdf2339436a816a0d9e45767664).**

## Getting ready for the challenge

For this challenge, in addition to the concepts seen in class, we will use some new things to make our application even better. So, before going directly to the challenge code, we'll explain a little bit about Fake API with JSON Server.

### Fake API with JSON Server

Just as we used MirageJS in module 2 to simulate an API with transaction data from the dt.money application, we are going to use JSON Server to simulate an API that has information about genres and movies.

Navigate to the created folder, open it in Visual Studio Code and execute the following commands in the terminal:

```bash
yarn
yarn server
```

Then you will see the message:

<img src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F1abc3356-2936-4106-a4fe-a3fc8efd1373%2FUntitled.png?table=block&id=7fe88f6f-62c6-45c7-a898-d1672dbbe6bd&width=1420&userId=c2f20f93-e6f2-4785-879d-55dde28c4d2e&cache=v2">

Note that it started a fake API with `/genres` and `/movies` resources on `localhost` on port `3333` from the information in the file [server.json](https://github.com/rocketseat-education/ignite-template-componentizing-a-application/blob/main/server.json) located at the root of your project. Accessing these routes in your browser, you can see the return of the information already in JSON (by double-clicking, the image will expand):

<img src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F12a3c689-264b-4bd4-8515-730dfe8dd407%2FUntitled.png?table=block&id=e27d872a-13a6-4c37-ba61-34b7fb2f74dd&width=850&userId=c2f20f93-e6f2-4785-879d-55dde28c4d2e&cache=v2">
<img src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F400b84d4-2de4-4cd3-aef2-139f3103e9f6%2FUntitled.png?table=block&id=c2e1b5cd-c028-45b6-9319-b88aab9b0ece&width=670&userId=c2f20f93-e6f2-4785-879d-55dde28c4d2e&cache=v2">

That way, it's enough to consume these API routes normally with Axios. If you want to study more about **JSON Server**, take a look [aqui](https://github.com/typicode/json-server).

## What should I edit in the application?

With the template already cloned, the dependencies installed and the [fake API rodando](https://www.notion.so/Desafio-01-Criando-um-hook-de-carrinho-de-compras-5769216778794019a83f544e79167b12), you must create **at least** the SideBar and Content components that already have the files created.
The files to be edited are:

- **src/App.tsx**
  This component contains the entire application with the exception of the `Button` component which does not need to be changed and the `Icon` which also does not need to be changed.
- **src/components/Content.tsx**
  This component, still empty, must have all the logic and body responsible for the application header and content (section outlined in red):

<img src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fff7c8a12-50d1-4a20-a680-9085d0bd6823%2Fexample.png?table=block&id=641fa56e-763e-48f3-8a2b-1bf93007de1b&width=1250&userId=c2f20f93-e6f2-4785-879d-55dde28c4d2e&cache=v2">

- **src/components/SideBar.tsx**
  This component, also empty, must have all the logic and body responsible for the section that contains the website title and the navigation part on the left of the page (section outlined in red):

<img src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F88f057c2-d29a-4b0d-b9ed-f11385e09030%2Fexample.png?table=block&id=673530e2-c5dc-4813-97f2-37c4dfabc170&width=1340&userId=c2f20f93-e6f2-4785-879d-55dde28c4d2e&cache=v2">

If you prefer, you can also component some other parts of the application, such as the header, but this is not a requirement of this challenge 🚀


## How should the application look at the end?

Are you in doubt (or curious 👀) to see what the application should look like at the end of the challenge? we leave this [![Watch the video]](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/10783a0f-e3a7-4991-8bb5-43f73508431f/demo.mp4?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45O3KS52Y5%2F20211104%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20211104T140248Z&X-Amz-Expires=86400&X-Amz-Signature=0eeda58a3feaa62dd7368763defc1930e55741d4e9db01a00b914dc9825a5d51&X-Amz-SignedHeaders=host) showing the main features you should implement to help you (or kill your curiosity 👀).

# 📅 Delivery

This challenge must be delivered from the Rocketseat platform. Submit the link to the repository where you made your changes. After completing the challenge, in addition to sending the code to GitHub, posting on LinkedIn is a good way to demonstrate your knowledge and efforts to advance your career for future opportunities.

## 📖 [Notion](https://www.notion.so/Desafio-02-Componentizando-a-aplica-o-b9f0f025c95b437699d0c3115f55b0f1)
© 2021 GitHub, Inc.
Terms
Privacy
Security
Status
Docs
Contact GitHub
Pricing
API
Training
Blog
About
