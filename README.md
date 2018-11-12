<p align="center">
	<a href="https://travis-ci.org/eoscostarica/dmeetup">
		<img src="https://travis-ci.org/eoscostarica/dmeetup.svg?branch=master" alt="TravisCI">
	</a>
	<a href="http://standardjs.com">
		<img src="https://img.shields.io/badge/code%20style-standard-brightgreen.svg" alt="StandardJS">
	</a>
	<a href="https://git.io/col">
		<img src="https://img.shields.io/badge/%E2%9C%93-collaborative_etiquette-brightgreen.svg" alt="Collaborative Etiquette">
	</a>
	<a href="https://discord.gg/bBpQHym">
		<img src="https://img.shields.io/discord/447118387118735380.svg?logo=discord" alt="chat on Discord">
	</a>
	<a href="https://twitter.com/intent/follow?screen_name=eoscostarica">
		<img src="https://img.shields.io/twitter/follow/eoscostarica.svg?style=social&logo=twitter" alt="follow on Twitter">
	</a>
	<a href="#">
		<img src="https://img.shields.io/dub/l/vibe-d.svg" alt="MIT">
	</a>
</p>

<p align="center">
	<a href="https://eoscostarica.io">
		<img src="https://cdn.rawgit.com/eoscostarica/assets/574d20a6/logos/eoscolors-transparent.png" width="300">
	</a>
</p>
<br/>
<p align="left">
	<img src="brand/logo/logo.svg" width="300px">
</p>

A decentralized platform and economic system that rewards community members for organizing and attending meetups and workshops. You will be able to build a reputation, get rewarded and charge a fee in crypto. 

It's a decentralized version of [Meetup](https://meetup.com) with token incentives for the members.  
A version of [Steemit](https://steemit.com) for events and workshops.

## Contents

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->

- [Getting Started](#getting-started)
- [Whitepaper](#whitepaper)
- [Contributing](#contributing)
- [Project Directory Structure](#project-directory-structure)
- [React App Documentation](#react-app-documentation)
  - [Start Up](#start-up)
- [Continuous Integration Process](#continuous-integration-process)
- [Why EOS ?](#why-eos-)
- [EOS.io Application Stack](#eosio-application-stack)
- [EOS Documentation & Resources](#eos-documentation--resources)
- [EOS Storage](#eos-storage)
- [IPFS Documentation](#ipfs-documentation)
- [About EOS Costa Rica](#about-eos-costa-rica)
- [License](#license)
- [Contributors](#contributors)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## Getting Started

dmeetup is an EOS dApp that allows people to organize meetups and workshops. 

It is a 100% open-source and community-driven project and we welcome contributions of all sorts. There are many ways to help, from reporting issues, proposing features, improving documentation, contributing code, design/ux proposals, refining the economic model and helping us improve our community.

The main communication channels for organizing and collaborating are this repository and the [EOS Costa Rica Discord server](https://discord.gg/bBpQHym). Feel to join and ask as many questions you may have.

At [learn.eoscostarica.io](https://learn.eoscostarica.io) you can find curated Blockchain and EOS learning resources. 

## Whitepaper

The whitepaper and economic model are a work in progress

* https://github.com/eoscostarica/dmeetup/issues/4
* https://github.com/eoscostarica/dmeetup/issues/27
* https://github.com/eoscostarica/dmeetup/blob/whitepaper/docs/whitepaper.md

## Contributing

We use a Kanban-style board with built-in triggers to automatically move issues and pull requests across New Issues, To Do, In Progress and Done columns. That's were we prioritize the work. [Go to Project Board](https://github.com/eoscostarica/dmeetup/projects/1).

We follow EOS Costa Rica's Open Source Contributing Guidelines. https://developers.eoscostarica.io/docs/open-source-guidelines

Our weekly sync call is every Monday 7pm-8pm Costa Rica / Central Standard Time at [meet.eoscostarica.io](https:/meet.eoscostarica.io).

Please report bugs big and small by [opening an issue](https://github.com/eoscostarica/dmeetup/issues).

## Project Directory Structure

```
.
├── docs/ .............................................. documentation files and media
├── brand/ ............................................. all branding and identity
├── services/ .......................................... documentation files and media
|	├── eosio/ ......................................... eosio blockchain service
|	|	├── config/ .................................... eosio service configuration
|	|	├── contracts/ ................................. dmeetup smart contracts 
|	└── frontend/ ...................................... reactjs frontend
|		├── public/ .................................... static and public files
|		├── src/ ....................................... reactjs views and components
|		├── config-overrides.js ........................ configuration overrides for `cra`
|		├── .env ....................................... environment variables
|		├── .eslintrc .................................. code style rules
|		└── package.json ............................... dependencies manifest
├── docker-compose.yaml ................................ docker compose for local dev
├── CONTRIBUTING.md .................................... contributing guidelines
├── LICENSE ............................................ project license
├── README.md .......................................... project homepage
├── netlify.toml ....................................... netlify configuration file
└── .travis.yml ........................................ travis ci configuration file
```

## React App Documentation

The React.js DApp was bootstrapped with [Create React App](https://github.com/facebookincubator/create-react-app).

See [full create-react-app documentation](docs/create-react-app.md)

[![Why React.js](https://monosnap.com/image/thWXLTTerX96Rnn8IhqujvNvlx5wa1.png)](https://www.youtube.com/watch?v=WsmgDnHOWh4)

### Start Up

1. `$ yarn`
2. `$ yarn start`

This will launch your browser or you can navigate directly to `http://localhost:3000/` to use dmeetup.

**ÐMeetup App Components**

- [react-app-rewired](https://github.com/timarney/react-app-rewired) for tweaking `create-react-app` configuration without ejecting
- [reach-router](https://github.com/reach/router) for a more accessible router.
- state management with [rematch](https://github.com/rematch/rematch) to use `redux` best practices without all the boilerplate.
- [grid-styled](https://github.com/jxnblk/grid-styled) for a flexbox grid built on top of `styled-components` and [system-components](https://github.com/jxnblk/styled-system/tree/master/system-components) for a consistent design system.

## Continuous Integration Process

We follow a continuous integration process based on Github flow that leverages the following tools:

- [TravisCI](https://travis-ci.org/) to run test and code style checks
- [Netlify](https://netlify.com) for continuous delivery to the stanging server and creation pull request specific environments for testing. awesome!
- [Code Factor](https://codefactor.io) for automated code quality reviews.


## Why EOS ?

[![Why EOS](https://monosnap.com/image/CDcIfufeYs0rJPH2viNkCJSPV6bY4O.png)](https://www.youtube.com/watch?v=3kqkTYqTvDA)

![EOS Network](https://github.com/eoscostarica/dmeetup/blob/master/docs/img/eos-network.jpg)

[![The REAL Difference Between Ethereum and EOS](https://monosnap.com/image/Asv5NiYI9Il7pUegy67KT6TqnqqPgN.png)](https://www.youtube.com/watch?v=YmwZ3xvIyN4)


## EOS.io Application Stack

![](https://github.com/eoscostarica/dmeetup/blob/master/docs/img/eos-application-stack.png)  
source https://steemit.com/eos/@eosio/introducing-eos-io-application-stack

## EOS Storage

- [5 Reasons Why EOS Storage Will Change Data Storage Forever](https://www.youtube.com/watch?v=7mFzb5SqS9U)
- [EOS.IO Storage White Paper](https://steemit.com/eos/@eosio/eos-io-storage-white-paper-now-available)

EOS Storage will allow you to host dApps thru EOS APIs, this hasn't been implemented yet, though.
In the mean time we are going to have use IPFS directly.

- https://ipfs.io/docs/
- https://github.com/ipfs/awesome-ipfs

## IPFS Documentation

- https://github.com/ipfs/ipfs#how-ipfs-work
- https://ipfs.io/docs/
- https://beta.docs.ipfs.io
- https://github.com/ipfs/js-ipfs

[![IFPS Simply Explained](https://monosnap.com/image/PW76DIRPGLOmtWyPEiXK2NvsDHiR4x.png)](https://www.youtube.com/watch?v=5Uj6uR3fp-U)

## About EOS Costa Rica

We challenge ourselves to provide the EOS platform with a strong geographical and political diversity by running the most robust EOS Block Producer possible from Costa Rica; We pledge to leverage our talent, experience, and sustainable internet resources to meet such an important challenge.

EOS Costa Rica supports the EOS.io community by maintaining and contributing to open source initiatives, meetups and workshops.

[eoscostarica.io](https://eoscostarica.io)

## License

MIT © [EOS Costa Rica](https://eoscostarica.io)  

## Contributors

Thanks goes to these wonderful people ([emoji key](https://github.com/kentcdodds/all-contributors#emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore -->
| [<img src="https://avatars0.githubusercontent.com/u/391270?v=4" width="100px;"/><br /><sub><b>Gabo Esquivel</b></sub>](https://gaboesquivel.com)<br />[🤔](#ideas-gaboesquivel "Ideas, Planning, & Feedback") [📖](https://github.com/eoscostarica/dmeetup/commits?author=gaboesquivel "Documentation") [💻](https://github.com/eoscostarica/dmeetup/commits?author=gaboesquivel "Code") [👀](#review-gaboesquivel "Reviewed Pull Requests") [📹](#video-gaboesquivel "Videos") [📢](#talk-gaboesquivel "Talks") | [<img src="https://avatars1.githubusercontent.com/u/1179619?v=4" width="100px;"/><br /><sub><b>Jorge Murillo</b></sub>](https://github.com/murillojorge)<br />[🤔](#ideas-murillojorge "Ideas, Planning, & Feedback") [📖](https://github.com/eoscostarica/dmeetup/commits?author=murillojorge "Documentation") [🎨](#design-murillojorge "Design") [💻](https://github.com/eoscostarica/dmeetup/commits?author=murillojorge "Code") [👀](#review-murillojorge "Reviewed Pull Requests") | [<img src="https://avatars2.githubusercontent.com/u/3157426?v=4" width="100px;"/><br /><sub><b>Kevin Wolf</b></sub>](https://github.com/kevinwolfcr)<br />[🤔](#ideas-kevinwolfcr "Ideas, Planning, & Feedback") [📖](https://github.com/eoscostarica/dmeetup/commits?author=kevinwolfcr "Documentation") [💻](https://github.com/eoscostarica/dmeetup/commits?author=kevinwolfcr "Code") [👀](#review-kevinwolfcr "Reviewed Pull Requests") | [<img src="https://avatars0.githubusercontent.com/u/5632966?v=4" width="100px;"/><br /><sub><b>Xavier Fernandez</b></sub>](https://github.com/xavier506)<br />[🤔](#ideas-xavier506 "Ideas, Planning, & Feedback") [📝](#blog-xavier506 "Blogposts") [📢](#talk-xavier506 "Talks") [🚇](#infra-xavier506 "Infrastructure (Hosting, Build-Tools, etc)") | [<img src="https://avatars2.githubusercontent.com/u/40245170?v=4" width="100px;"/><br /><sub><b>Edgar Fernandez</b></sub>](http://www.eoscostarica.io)<br />[🤔](#ideas-edgar-eoscostarica "Ideas, Planning, & Feedback") [📝](#blog-edgar-eoscostarica "Blogposts") [📢](#talk-edgar-eoscostarica "Talks") | [<img src="https://avatars2.githubusercontent.com/u/13205620?v=4" width="100px;"/><br /><sub><b>Rubén Abarca Navarro</b></sub>](https://github.com/rubenabix)<br />[🤔](#ideas-rubenabix "Ideas, Planning, & Feedback") [👀](#review-rubenabix "Reviewed Pull Requests") | [<img src="https://avatars1.githubusercontent.com/u/1449049?v=4" width="100px;"/><br /><sub><b>Friedger Müffke</b></sub>](https://github.com/friedger)<br />[💻](https://github.com/eoscostarica/dmeetup/commits?author=friedger "Code") [🐛](https://github.com/eoscostarica/dmeetup/issues?q=author%3Afriedger "Bug reports") [💡](#example-friedger "Examples") |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/kentcdodds/all-contributors) specification. Contributions of any kind welcome!
