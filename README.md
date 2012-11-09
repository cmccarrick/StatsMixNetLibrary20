StatsMixNetLibrary20
====================

Version to support the .Net 2.0 framework.

This version uses a version of the Mono library for JSON and RestSharp.

Here is an example to call using async in C# .Net 2.0.

If you do not neet async call one of the other methods directly.



    Thread t = new Thread(submitJob);
    t.Start();


    private void submitJob()
        {

            Client smClient = new Client("API_KEY");
            smClient.trackasync("METRIC_NAME", 1);

        }