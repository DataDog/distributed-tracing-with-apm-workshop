# Distributed Tracing with APM Workshop

This will be a follow up repo to my [2018 Dash APM Workshop](https://github.com/burningion/dash-apm-workshop), incorporating feedback from the event.

Specifically, this will add:

* Starting with Automatic Instrumentation, and a more complex example program
* More live traffic, to see Trace Search (announced at DASH)
* Debugging a bigger, more complex system, to showcase a more real world use case
* More Datadog UI usage
* More relevant examples and names for traces
* More realistic errors 
* ... and should also work in Windows.

In the meantime, unless otherwise noted, this repository is a work in progress. 

If you've stumbled upon it and have feedback, or have something you'd  like to see, feel free to create an issue.

# Running the Application

You'll need to have a Datadog account with APM and logging enabled. A free trial should work to play with.

```bash
$ POSTGRES_USER=postgres POSTGRES_PASSWORD=<pg password> DD_API_KEY=<api key> docker-compose up
```

You can then hit the API at `http://localhost:5000/status` and `http://localhost:5000/add_sensor` and look at your Datadog traces to see the distributed traces.