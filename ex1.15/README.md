# Here's a copy of the readme provided at docker hub:

Link to container in Docker Hub:
https://hub.docker.com/repository/docker/aahaavis/shakugenerator

This is a containerized version of a shakuhachi music generation software created as university course assignment.

The original project can be found at: https://github.com/ElectricShakuhachi/tiralabra-shakugenerator/blob/main/documentation/user_guide.md

The gist of how to run it:

    run the container by the command: docker run -it aahaavis/shakugenerator
    You will be prompted for type of output desired (wav, csv, midi) The output will be printed on the terminal in numerical form describing the lenghts and relative pitches generated. The output is generated in chosen format as a file into the container, under "/usr/src/app" as "tmp_wav_output.mid" or "tmp_midi_output.mid" (the current application doesn't generate csv for some reason, but the other two are functional, wav is generated with extension as ".mid" but it is in fact in wav format)
    the resulting files may be copied from the container with for instance: docker cp <container_id>:/usr/src/app/tmp_wav_output.mid
