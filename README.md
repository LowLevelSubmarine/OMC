# OMC
OpenMediaCommands is a standard for crossplatform media commands. Ranging from simple queueing instructions to viewing specific genres.

## Commands
#### VIEW/(c,a)
Display content or an artist
#### QUEUE_END/(c)
Add content to the end of the current queue
#### QUEUE_START/(c)
Add content to the start of the current queue
#### PLAY/(c)
Instantly play the given content
#### SKIP_NEXT
Skip to the next queue item
#### SKIP_PREVIOUS
Skip to the previous queue item

## Content identifier (content, c)
A song or a video
#### Specific: s-youtube.com-dQw4w9WgXcQ
Specific identifiers are made up of a source (for example "youtube.com") and the corresponding content id (for example "dQw4w9WgXcQ")
#### Generic: g-rick%20astley-never%20gonna%20give%20you%20up
Generic identifiers are made up of an escaped string with the artists name, followed by the contents name
_Example: content=s-youtube.com-dQw4w9WgXcQ~g-rick%20astley-never%20gonna%20give%20you%20up_

## Artist identifier (artist, a)
A musician or video creator
#### Specific s-spotify.com-0gxyHStUsqpMadRV0Di1Qt
Specfic identifiers are made up of a source (for example "spotify.com") and the corresponding artist id (for example "0gxyHStUsqpMadRV0Di1Qt")
#### Generic g-rick%20astley
Generic identifiers are made up of an escaped string with the artists name
_Example: artist=s-spotify.com-0gxyHStUsqpMadRV0Di1Qt~g-rick%20astley

## Escaping
The escaping works exactly like the url encoding with the addition, that "-" must be escaped to "%1B-" also.

## A note on genric identifiers
Generic idetifier are inconvinient to implement and therefore not recommended sending without another. Generic ids identify media independent from the platform.
