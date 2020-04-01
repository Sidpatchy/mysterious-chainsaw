# mysterious-chainsaw, a garden management tool.
I don't have the sensors I need yet, but I am here starting this nonetheless.

The overall goal for this project is to create a nice-looking (though that may come second), functional, and highly expandable system for monitoring my garden. The likeliness of that happening? Pretty low.

The current plan is to use something like Firebase or SQLite, if that doesn't work out, I will probably end up hosting a MySQL or MariaDB server on StormCloud (my servers) that this syncs to. It honestly depends on how big I decide to make this.

# Things that need to be done
1. Build a system that communicates with the database, reliably.

This will probably be built on Python as that's what I'm most familiar with, also, this project isn't super speed-dependent.

2. Design a system for sending data from the sensors to the database.

This will likely be integrated into the code that communicates with the database. It needs to generate enough data that I am able to create cool graphs without spending hundreds of hours designing it.

3. Design a website to generate oh so sexy graphs from the data stored on the database.

I would much like to go the Octoprint route and have everything stored on one device rather than force myself to keep two devices running at once. Ideally I will offer support for many digital sensors, the only issue is my budget for doing something like this is very limited. 

# Key goals
Eventually, I would like to expand this into something bigger that other people contribute to (mainly more sensor configs). To achieve that, I need to build a solid framework that doesn't get in the way of people and their project. Next, I need to ensure that this project stays highly modular. It's unfortunate, but I can't just have one file that does everything anymore. I need to have a base for the website, a base for reading sensors, and a base for the database. Ideally, it will be able to work with and without the three.

I mentioned Octoprint earlier and I would like to create something similar to its plugin repo at some point. Perhaps compatibility for sensors could be added via that, the software would need to be shipped with common configs for sensors but it should also have tools that allow users to add their own sensors and submit them to the repo.

### I am probably biting off way more than I can chew :(
