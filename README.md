# depth-Nerf-project
our goal for this project is to convert the nerf code " that create rgb video(3D) from 
2D rgb image input "by use rgb loss, to depth  nerf code "that create depth video (3D) from 2D rgb image input  " , by use depth loss.

- at the orginal nerf code we dont have the truth depth image " so we have problem
 to calculate the depth loss",so we solve it by :
in section of training of model we do two training loop, at first training  loop
we do the training by use rgb loss " difference between rgb image that nerf model create with the rgb image input  ", after the all iterations of the trainig we make the nerf model create the depth image and save it an array to use it in the second training loop.
at the second training loop we take the depth images that we save in the array at first training loop to be the target_depth, and now we do the training by use depth loss "difference between depth image that nerf model  create with the target_depth"

. RUNNING CODE :
we run the code by using google colab.



