Today's post shows you how you can connect multiple parties to the same call using the Vonage Voice API.

If you read our earlier post on how to receive inbound calls, you will see that this example is very similar: it defines a webhook endpoint that Vonage's APIs can make a request to when someone calls your virtual number. As before, its response is a Nexmo Call Control Object (NCCO) that tells Vonage how to handle the call.

But this time, in addition to the talk action for playing text-to-speech to the caller, you will use a conversation action in the NCCO to start a conference call. The first person to call the number initiates the conference. Subsequent callers are able to hear and talk to the other participants.

The complete source code is available on GitHub.
