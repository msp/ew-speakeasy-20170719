# Pattern generation in Tidal Cycles: live coding emergent audio

## Define: Emergent behaviour


In philosophy, systems theory, science, and art, emergence is a phenomenon
whereby larger entities arise through interactions among smaller or simpler
entities such that the larger entities exhibit properties the smaller/simpler
entities do not exhibit.

The butterfly effect is the concept that small causes can have large effects.
Initially, it was used with weather prediction but later the term became a
metaphor used in and out of science.


## Define: Tidal Cycles

TidalCycles (or Tidal for short) is a language for live coding patterns.
It allows you to make musical patterns with text, describing sequences and
ways of transforming and combining them, exploring complex interactions
between simple parts.

#### Pattern Generation

Tidal is a Domain Specific Language written in Haskell. Declarative language for describing patterns, transformations and effects.

#### Pattern Composition

Tidal is highly composable in that pattern transformations can be easily combined together, allowing you to quickly create complex patterns from simple ingredient.

#### Text Interface

Tidal does not make sound itself, but is designed for use with the SuperDirt synth, and can control other synths over Open Sound Control or MIDI.

### Architecture

<pre>
+-------------------------------------+                                
|                                     |                                
|                                     |                                
|                                     |                                
|                                     |                                
|                                     |                                
|                ATOM                 |                                
|                                     |                                
|                            +--------+                                
|                            |        |                                
|                            |TIDAL   |                                
|                            |PLUGIN  |                                
|                            |        |                                
+----------------------------+--------+                                
                  |                                                    
                  |                                                    
+-------------------------------------+                                
|               HASKELL               |                                
+-------------------------------------+                                
                  |                                                    
                  |  OSC MESSAGES                                      
                  |                                                    
                  |                                                    
+-------------------------------------+                                
|                                     |                                
|                                     |                                
|                                     |                                
|                                     |                                
|                                     |                                
|            SUPER COLLIDER           |                                
|                                     |                                
|                           +---------+                                
|                           |SUPERDIRT|                                
|                           |         |                                
|                           |SAMPLER  |                                
|                           |         |                                
+---------------------------+---------+                                
</pre>

## Define: Supercollider

SuperCollider is an environment and programming language originally released in 1996 by James McCartney for real-time audio synthesis and algorithmic composition.
