    
    docker build -t python-3.11-ffmpeg .

    docker run -it python-3.11-ffmpeg bash

    ffmpeg -buildconf

    docker tag d137061904e2 cicybot/python-3.11-ffmpeg:1.0.1
    docker tag d137061904e2 cicybot/python-3.11-ffmpeg:latest   

    docker logout
    docker login

    docker push cicybot/python-3.11-ffmpeg:1.0.1
    docker push cicybot/python-3.11-ffmpeg:latest