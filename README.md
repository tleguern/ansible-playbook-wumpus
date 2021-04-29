# Ansible Playbook: Hunt the Wumpus

This project is an attempt at porting the old computer game `Hunt the Wumpus` written by Gregory Yob in 1973 to Ansible.
The work is still in progress.

Here is a list of intended features for first release:

- [ ] Generate a random dodecahedron ;
- [ ] Generate a random position for the bats ;
- [ ] Generate a random position for the pits ;
- [ ] Generate a random position for the Wumpus ;
- [X] Move around the map ;
- [X] Bats transport the player ;
- [X] Death by falling in a pit ;
- [X] Death by being eaten by the evil Wumpus ;
- [X] Death by firing the last arrow ;
- [X] Feeling nearby pits ;
- [X] Hearing nearby bats ;
- [X] Smelling nearby wumpii ;
- [ ] Shoot arrows ;
- [ ] Random chances that the arrow fail after 4 rooms ;
- [ ] The Wumpus awakens and moves on shot failure ;

Features not fit for the first release:

- [ ] Difficulty selection ;
- [ ] Generation of different shapes of cave as in `Hunt the Wumpus II`;
- [ ] Add _tumaeros_: anaerobic termite, arrows eaters ;
- [ ] The player can survive walking on a pit (1/6) ;
- [ ] The Wumpus can awaken and move on bumping walls (1/6);

## Caveats

- The cave is not randomly generated yet ;
- Debug information comprising a full map of the cave are shown each turn ;
- The starting position is not validated before starting so there is 1/10 chances to start in a pit and 1/20 to start on the evil Wumpus ;
- Add the aenerobu 

## License

ISC

## Contributing

[Send patches on SourceHut](https://lists.sr.ht/~tleguern/misc).

## Author Information

Tristan Le Guern <tleguern@bouledef.eu>
