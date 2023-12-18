## Vectrex (with pong)

This is a pong clone for the Vectrex. It was written primarily to build a good pipeline and codebase for developing Vectrex games in C++. It started from [Joakim Larsson's VectrexTutoial](https://github.com/JoakimLarsson/VectrexTutorial), then some issues were fixed building with C++, and improved the Makefile for multi-source projects. Fixes by [Malban/PeerC](http://vectrexc.malban.de/) were also integrated.

### Building

The easiest way to build the game is to use the [docker](https://github.com/cartheur/M6809-vectrex-docker) image with the `gcc6809` cross-compiler and dev tools:

```bash
docker pull cartheur/gcc6809
git clone https://github.com/cartheur/M6809-vectrex.git
cd vectrex-pong
docker run -v $(pwd):/root/vectrex-pong -t -i cartheur/gcc6809 make -C vectrex-pong
```

**Note:** On Windows (using Docker Desktop), replace ```$(pwd)``` with ```%cd%```.

### Detailed instructions

Can be found on the companion [github](https://github.com/cartheur/M6x09-gcc6809) project.