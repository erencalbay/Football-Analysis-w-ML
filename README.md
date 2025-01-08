# Football Analysis with Machine Learning

This project uses machine learning and computer vision techniques to analyze football matches. The project processes video data to perform various analyses such as player and ball tracking, team assignments, camera movement estimation, and speed/distance calculations.

![Football Analysis Detection System](/docs/image/football.png)
## Features

- **Player and Ball Tracking**: Tracks players and the ball in the video.
- **Team Assignments**: Assigns players to their respective teams.
- **Camera Movement Estimation**: Estimates camera movements and adjusts tracking data accordingly.
- **View Transformation**: Transforms tracking data to a different view.
- **Speed and Distance Calculations**: Calculates the speed and distance covered by players.

## Installation

1. Clone this repository:
    ```bash
    git clone https://github.com/yourusername/Football-Analysis-w-ML.git
    cd Football-Analysis-w-ML
    ```

2. Install the required Python packages:
    ```bash
    pip install -r requirements.txt
    ```


3. For the most reliable object detection with YOLO, which is required for analysis, you can download the football players detection dataset via Roboflow and create the best model yourself with the [football_training_yolo_v5]() file, or you can obtain the model ready-made.


## Usage

1. Run the [main.py](http://_vscodecontentref_/2) file to start the analysis:
    ```bash
    python main.py
    ```

2. The analysis results will be saved in the [output_videos](http://_vscodecontentref_/3) directory.

## File Structure

- [main.py](http://_vscodecontentref_/4): The main script to run the analysis.
- [utils](http://_vscodecontentref_/5): Utility functions and tools.
- [trackers](http://_vscodecontentref_/6): Tracking algorithms.
- [team_assigner](http://_vscodecontentref_/7): Team assignment algorithms.
- [player_ball_assigner](http://_vscodecontentref_/8): Player and ball assignment algorithms.
- [camera_movement_estimator](http://_vscodecontentref_/9): Camera movement estimation algorithms.
- [view_transformer](http://_vscodecontentref_/10): View transformation algorithms.
- [speed_and_distance_estimator](http://_vscodecontentref_/11): Speed and distance calculation algorithms.

## Modules and Functions

### [main.py](http://_vscodecontentref_/12)

The main script that performs the following steps:
- Reads the video
- Initializes the tracker
- Performs object tracking and position determination
- Estimates and adjusts for camera movement
- Transforms the view
- Interpolates ball positions
- Calculates speed and distance
- Assigns players to teams
- Assigns ball possession
- Generates and saves the output video frames

### [utils](http://_vscodecontentref_/13)

Contains utility functions and tools. For example:
- `read_video`: Reads a video file and splits it into frames.
- `save_video`: Combines frames and saves them as a video file.

### [trackers](http://_vscodecontentref_/14)

Contains tracking algorithms. For example:
- `Tracker`: Performs object tracking and position determination.

### [team_assigner](http://_vscodecontentref_/15)

Contains team assignment algorithms. For example:
- `TeamAssigner`: Assigns players to their respective teams.

### [player_ball_assigner](http://_vscodecontentref_/16)

Contains player and ball assignment algorithms. For example:
- `PlayerBallAssigner`: Assigns the ball to players.

### [camera_movement_estimator](http://_vscodecontentref_/17)

Contains camera movement estimation algorithms. For example:
- `CameraMovementEstimator`: Estimates camera movements and adjusts tracking data accordingly.

### [view_transformer](http://_vscodecontentref_/18)

Contains view transformation algorithms. For example:
- `ViewTransformer`: Transforms tracking data to a different view.

### [speed_and_distance_estimator](http://_vscodecontentref_/19)

Contains speed and distance calculation algorithms. For example:
- `SpeedAndDistance_Estimator`: Calculates the speed and distance covered by players.