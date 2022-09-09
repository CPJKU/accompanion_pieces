# ACCompanion Scores and Material

This is a repo that contains pieces, scores and performances for playing with the accompanion.
It is mainly used as a sub-module at the ACCompanion repo.

## Organization

The repository is divided into two folders/categories:
 - Simple Pieces
 - Complex Pieces

The division has nothing to do with complexity of the music but only with the number of related material we need to feed to the ACCompanion.
As a rule of thumb, the indispensable information in both categories is a score with a primo and a second part.

### Simple Pieces

The simple pieces can contain only the score with a primo and a second part. Furthermore, the Primo part needs to be mostly monophonic.
The simple pieces can contain additional information such as a pdf and/or a musescore file of the score.
Here we save pieces that will use the simple HMM follower.

### Complex Pieces

The header Complex does not refer on the complexity of the music but only on the material we need to provide.
Pieces saved here need to have 3 categories/folders of information:

1. **musicxml** - The score with a primo and secondo part.
2. **match** - Primo and Secondo alignments between performances and the score.
3. **basismixer** - A basismixer rendition of the secondo. 



## Adding a New Piece

To add a new piece you will need to provide the same material as in the corresponding folders.
Please try to keep the naming of the folders and the files consistent.

#### Simple Piece Example

```
accompanion_pieces
|	complex_pieces
└───simple_pieces
|	└─── new_piece
|		|	primo.musicxml
|		|	secondo.musicxml
|		| 	score.pdf
```



#### Complex Piece Example

```
accompanion_pieces
|	simple_pieces
└───complex_pieces
|	└─── new_piece
|		└─── musicxml
|			|	primo.musicxml
|			|	secondo.musicxml
|			|	score.pdf
|		└─── match
|			└─── primo
|				|	new_piece_performance_primo_1.match
|				|	new_piece_performance_primo_2.match
|				|	...
|			└─── secondo
|				|	new_piece_performance_secondo_1.match
|				|	new_piece_performance_secondo_2.match
|				|	...
|		└─── basismixer
|			|	bm_new_piece.match
```

