docker-openrefine
=================

Run the docker
--------------

This docker is hosted on the [official docker.io hub][5]. Running it is as simple as:

    docker run -p 80:3333 alexszilagyi/openrefine

If you want refine projects to be persistent, you must mount `/mnt/refine` as follows:

    docker run -p 80:3333 -v /path-to-host:/mnt/refine alexszilagyi/openrefine

You can also increase the max size of the heap, by specifying the REFINE_MEMORY environment variable:

    docker run -p 80:3333 -e REFINE_MEMORY=24G alexszilagyi/openrefine

[5]: https://registry.hub.docker.com/u/spaziodati/openrefine/
