This project was created as part of experimenting with Gemini. You can create a template project with new Android studio by following the steps.

While running the project , it was not working right away as AI model used in the template project was deprecated. I had to update the file BakingViewModel as you can see below


private val generativeModel = GenerativeModel(
        modelName = "gemini-1.5-flash-latest",
        apiKey = BuildConfig.apiKey,
        requestOptions = RequestOptions(apiVersion = "v1beta")
    )
