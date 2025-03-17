Yoga Pose Detection and Correction College Project
Adding new poses
Preferably the images should be JPG/JPEG and the image names should be [number].jpg.

Create a new directory in ./poses_dataset/Images (the name can be anything but I recommend to use the name of the pose) and populate it the with the pose images.
Create another directory in ./poses_dataset/angles (folder name should be the same as what was used in step 1) and put one image of the pose. The image in this directory will be used as a 'known good' pose angles (the pose should be perfect), as in, during live detection the user's pose will be compared against this pose to make recommendations.
Run create_poses_csv.ipynb in the virtual env. This will create a file named https://github.com/bourbonbourbon/yoga-pose-detection-correction/blob/main/create_poses_csv.ipynb?short_path=1#L120 (you can name it whatever) which has all the x, y, z, and visibility values of all the desired landmark points of all poses in the ./poses_dataset/Images directory. The pose column value in the generated csv file will be an integer.
Then run create_angles_csv.ipynb. This will create another csv named https://github.com/bourbonbourbon/yoga-pose-detection-correction/blob/main/create_angles_csv.ipynb?short_path=1#L104 It will have the 'known good' pose angles.
Then run rfc_model.ipynb which uses the csv generated in the step 3 as the input file to train/test the data on. It will then create a .model file named https://github.com/bourbonbourbon/yoga-pose-detection-correction/blob/main/rfc_model.ipynb?short_path=1#L44
Change these variables in live_detection.py https://github.com/bourbonbourbon/yoga-pose-detection-correction/blob/main/live_detection.py#L106 https://github.com/bourbonbourbon/yoga-pose-detection-correction/blob/main/live_detection.py#L108 to whatever you have created in steps 4 and 5.
Finally change this dictionary to match whatever pose names you want. https://github.com/bourbonbourbon/yoga-pose-detection-correction/blob/main/live_detection.py#L26
Notes: Refer https://github.com/bourbonbourbon/yoga-pose-detection-correction/tree/1c9a4e50c00be9a8b677632901e6b8b0c459b6f4 for project structure.

Setup
Create a python virtual environment.
Activate the venv.
Install all the libraries from requirements.txt using pip install -r requirements.txt.
Plug in a camera.
Run the command python live_detection.py.
Stand in a well lit room.
Stand in a way such that you are completely in frame.
