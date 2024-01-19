---
icon: terminal
order: E
---

# Tensorboard

Tensorboard is a series of graphs where we can monitor the progress of our model during training, but there are many graphs. We are only interested in the graph called 'g/total'. You can find this by clicking on 'inactive' and selecting 'scalars'. Then, go to the last page, where you will find it in the last graph.

## How tu use it?
1. Open TensorBoard by running the following command in your terminal or use the run-tensorboard.bat file:

   ```
   tensorboard --logdir=path/to/your/logs
   ```

   Replace "path/to/your/logs" with the actual path to your TensorBoard logs.

2. Once TensorBoard is running, open your web browser and navigate to `http://localhost:6006` (or the address indicated in your terminal).

3. Click on the "Scalars" tab in TensorBoard.

4. Look for the "g/total" metric at the top to monitor the progress of your training.

![TensorBoard Screenshot](https://cdn.discordapp.com/attachments/1139925179489853470/1178729423411884152/image.png)

This image provides a visual guide for locating the "g/total" metric within the "Scalars" tab.
