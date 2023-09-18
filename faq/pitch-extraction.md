# Pitch extraction differences

- **pm:** It provides a quick but inefficient result and is less faithful to the voice model.

- **Harvest:** It offers a better replication of tones from our Acapella but is slower and often gives errors initially.

- **Dio:** Possibly used for moments when our Acapella has rapid word pronunciation, such as in rap.

- **Crepe:** It provides better word pronunciation results.

- **Crepe-tiny:** Similar to crepe, it processes faster but with less aggressiveness.

- **Mangio-crepe:** It provides better results in terms of breaths and performs the same as crepe, but it is slower and sometimes yields poorer results.

- **Mangio-crepe-tiny:** Similar to mangio-crepe, it's faster but with less aggressiveness.

- **Rmvpe:** It is a combination of pm and crepe but is fast for both training and inference. It is the most faithful to the voice model (currently the best option).