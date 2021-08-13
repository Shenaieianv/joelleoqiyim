# BBCS-X-NoSQL




Hello! Welcome to BuildingBloCS 2020 NoSQL Workshop!

For this workshop, we would be using:
- [MongoDB](https://www.mongodb.com) as a remote server database for storing our data
- [Gitpod](https://www.gitpod.io) as a online environment to run our code (as gitpod allows for some usage of terminal commands which we will be using later for importing our json file to the MongoDB server)

---

Before we begin, we would need to download MongoDB. In order to do this in Gitpod, we would need to configure  `.gitpod.dockerfile ` and `.gitpod.yml` files to use the dedicated MongoDB image built on top of gitpod/workspace-full.

Simply add the following line to .gitpod.dockerfile:

```
FROM gitpod/workspace-mongodb
```

Add the following line to .gitpod.yml:

```image:
  file: .gitpod.dockerfile
```
  
Note: if you are doing this locally you can [download the MongoDB Community Edition here](https://docs.mongodb.com/manual/administration/install-community/)

If you fork this repository, please ignore the lines above as the `.gitpod.dockerfile ` and `.gitpod.yml` files have already been configured before hand.

Optional: Storing MongoDB’s data inside /workspace ensures that it will get backed up and restored properly when you stop and restart a workspace, or share a snapshot. Note this repository is not configure to do so (and will not be covered in the workshop). [Click here for instructions](https://www.gitpod.io/blog/gitpodify/#running-init-scripts)


---

Next, edit README.md and change the `<username>`in the following line of markdown to your Github username such that you can click the button to open Gitpod.

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/joelleoqiyi/BBCS-X-NoSQL)

Once you changed README.md, click the button above.

---

Once Gitpod is fully loaded, you would need to do a few things before starting out on the workshop:
- Install `dnspython` package through the terminal in Gitpod
  ```
  pip install dnspython
  ```
- Install `pymongo` package through the terminal in Gitpod
  ```
  pip install pymongo
  ```
- Check for the version of `MongoDB` (as well as whether it is in your workspace)
  ```
  mongod --version
  ```
  you should get a result similar to: 
  ```
  db version v4.0.18
  git version: 6883g8d9j7f32176b1fd176df04da9165fd67
  OpenSSL version: OpenSSL 1.1.1d  10 Sep 2019
  allocator: tcmalloc
  modules: none
  build environment:
      distmod: ubuntu1804
      distarch: x86_64
      target_arch: x86_64
  ```

---

####That should be all the set-up needed for Gitpod for this workshop!!! :relaxed: 

**Full workshop steps will be written here after the workshop on 13th May 2020 (slides will be attached as well)**
