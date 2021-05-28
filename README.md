# Ansible Playbook: Hunt the Wumpus

This project is an attempt at porting the old computer game `Hunt the Wumpus` written by Gregory Yob in 1973 to Ansible.
If you do not know this piece of gaming history have a look at [the Wikipedia article](https://en.wikipedia.org/wiki/Hunt_the_Wumpus) about it or the [two](https://www.filfre.net/2011/05/hunt-the-wumpus-part-1/) [articles](https://www.filfre.net/2011/05/hunt-the-wumpus-part-2/) written by Jimmy Maher AKA The Digital Antiquarian.
In-game texts come from the [historic BSD port](http://bxr.su/search?q=wump.c&defs=&refs=&path=&project=DragonFly&project=FreeBSD&project=NetBSD&project=OpenBSD).

The goal is to navigate your way inside a strange cave with ever wrapping tunnels filled with hazards such as bottomless pits, giant bats and the awful, evil Wumpus.
This terrible, sucker footed creature sleeps somewhere in the cave, awaiting an adventurer fool enough to wander in its lair.
His teeth are long and sharp, quite adapted for a carnivore.
Fortunately you are equipped with magically enhanced crooked arrows able to fly in strange directions and even turn around.

Be careful not to shoot yourself!

## How to play

The following packages are necessary:

- ansible
- python-jmespath

Simply run the following command:

```sh
$ ansible-playbook wumpus.yml
...
```

There are two possible actions: `move` to an adjacent room (be careful about bottomless pits, giant bats or the occasional Wumpus) or `shoot` a crooked arrow to a series of rooms.

Here is an asciicast recording of a losing session:

[![asciicast](https://asciinema.org/a/Glv8slBLl0DzKC3xLanwKfdag.svg)](https://asciinema.org/a/Glv8slBLl0DzKC3xLanwKfdag)

## TODO

Here is a list of features yet to be implemented:

- [ ] Random chances that the arrow fail after 3 rooms ;
- [ ] Bats can drop player on other bats.
- [ ] Generation of different shapes of cave as in `Hunt the Wumpus II` ;
- [ ] Add _tumaeros_: anaerobic termite, arrows eaters ;
- [ ] The player can survive walking on a pit (1/6) ;
- [ ] The Wumpus can awaken and move on bumping walls (1/6) ;
- [ ] Difficulty selection ;

## Caveats

Ansible is not exactly a comfortable medium to play.
Consider yourself warned.

## License

ISC

## Contributing

Either send [send GitHub pull requests](https://github.com/tleguern/ansible-playbook-wumpus) or [send patches on SourceHut](https://lists.sr.ht/~tleguern/misc).

## Author Information

Tristan Le Guern <tleguern@bouledef.eu>
