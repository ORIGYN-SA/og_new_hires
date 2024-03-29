# Origyn Starter

### Puropose

This repo holds important information to provide to new Origyn Developers that will help them get up to speed.

### Usage

Welcome to your new og_new_hires project. This template has been customized with Motoko, Connect2IC, React and Material UI.

To get started, you might want to explore the project directory structure and the default configuration file. Working with this project in your development environment will not affect any production deployment or identity tokens.

To learn more before you start working with og_new_hires, see the following documentation available online:

- [Quick Start](https://smartcontracts.org/docs/current/developer-docs/quickstart/hello10mins)
- [SDK Developer Tools](https://sdk.dfinity.org/docs/developers-guide/sdk-guide.html)
- [Motoko Programming Language Guide](https://smartcontracts.org/docs/current/developer-docs/build/languages/motoko/)
- [Motoko Language Quick Reference](https://sdk.dfinity.org/docs/language-guide/language-manual.html)
- [Connect2IC](https://connect2ic.github.io/docs/)
- [JavaScript API Reference](https://erxue-5aaaa-aaaab-qaagq-cai.raw.ic0.app)
- [React Reference](https://reactjs.org)
- [Material UI](https://mui.com/material-ui/getting-started/installation/)

## Requirements

- Install the Internet Computer SDK

```
    sh -ci "$(curl -fsSL https://sdk.dfinity.org/install.sh)"
```

- NodeJS >=16.0.0
  Note: Make sure your node version is any version of 16 otherwise you may run into issues.

## Get Started

With Git and credentials:

```
git clone https://github.com/ORIGYN-SA/og_new_hires.git
```

With Git and SSH:

```
git clone git@github.com:ORIGYN-SA/og_new_hires.git
```

With NPM:

```
cd og_new_hires
npm install
```

## Running the project locally

If you want to test your project locally, you can use the following commands:

```bash
# Starts the replica, running in the background
dfx start --background

# Deploys your canisters to the replica and generates your candid interface
dfx deploy
```

Additionally, if you are making frontend changes, you can start a development server with

```bash
npm run dev
```

Which will start a server at `http://localhost:3000`, proxying API requests to the replica at port 8000.

## Origyn new hires project

Once you have the project running these are your tasks:

Important note: Make sure you read the project first including the challenge, the extra mile and how to submit the project. You may want to start from branching out and by adding Typescript functionality from the beggining.

- Inspect the project structure. On the backend folder you have 3 canisters running (droute, starter, welcome). These are your smart contracts written in Motoko.
- Try to understand Motoko syntax and the functions for each canister.
- Enter the following from the command line on the root directory of the project and see the response

```
dfx canister call starter hello
```

```
dfx canister call starter greet '("Hello from command line")'
```

- Create your own Motoko function in the starter canister and call it from the command line (note that after you create your function on starter canister you will need to recompile the canister. Hint: dfx deploy)
- Inspect front end directory and the components
- Inspect each individual component that interacts with the backend under the view folder
- Understand how we call the backend canister and the functions
- Create your own component to call your function

### Project challenge:

- Create a Motoko function that returns a list of things to do
- Create a view component with React and show the list
- With React filter the list with any attribute you prefer

### Go the extra mile - the super challenge :)

- Add functionality to the project to work with Typescript
- Do the project challenge in Typescript

### How to submit the project?

- Create a new repo on your github and push the project there
- Send an email to Fernando (you already have my email) with the project's link
