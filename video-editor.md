                                    Video editor idea

    This idea is a contuation of my phase 2 project.    
    MPV would include.
        While watching basketball videos the user will be able to Enter a play into the play table that
         includes a unique id, a project id, a team level, a game name, a quarter, start time stop time, play type, jersey number
         , assisting jersey # quality rating and special note and used status.

        Plays will be stored in a play table that can be sorted by used, player, game and play type.

        players, play type and games will have a used count.

        stretch goals will include adding a video aspect that will store the following in the Public folder
            -still photos.
            -entire games as a video file
            -indivual play clips ranging from the indexed start time,  stop time.
            -a running project which will be a single video of concanted video plays in the order that they were selected for use.

                Videos would be connected to the back end using the vidPy frame work.

                    Install(ubuntu)
                    
                        Install melt: sudo apt-get install melt
                        Install VidPy: pip install vidpy

                    Setup

                        from vidpy import config
                        config.MELT_BINARY = '/path/to/melt'
                        from vidpy import Clip, Composition

                Connecting to Python 


                        # start playing clip one after 1.5 seconds
                        clip1 = Clip('video.mp4', offset=1.5)

                        clip2 = Clip('anothervideo.mp4')
                        clip2.set_offset(5) # start clip2 after 5 seconds

                        composition = Composition([clip1, clip2])
                        composition.save('output.mp4')


                Connecting videos to front end

                        I would be using the framework React-player

                        install

                            npm install react-player

                        code example 


                            import React from 'react';
                            import ReactPlayer from 'react-player';

                            function VideoPlayer() {
                            return (
                                <ReactPlayer
                                url="<https://www.youtube.com/watch?v=ysz5S6PUM-U>"
                                width="640"
                                height="360"
                                controls
                                />
                            );
                            }

                            export default VideoPlayer;



Schema
![alt text](image.png)