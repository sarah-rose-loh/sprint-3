When you resize the screen to less than 550 px then the element rearrange themselves so they they are stacked one on top of the other rather than aligned horizontally. The margins also change.

I believe this is because of the command below. Which means that when the screen reachs the min width of 550px then elements in the container class take up 80% the width of the screen. I'm not sure if you need an instruction to stuck these.

/* For devices larger than 550px */
@media (min-width: 550px) {
  .container {
    width: 80%; }
  .column,
  .columns {
    margin-left: 4%; }
  .column:first-child,
  .columns:first-child {
    margin-left: 0; }