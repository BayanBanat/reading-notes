# Read: Class 16
## Serverless Functions
**Reading Questions :**

1.
   * Compared to traditional server-based architectures, serverless computing offers increased simplicity, scalability, cost efficiency, and faster time to market. It shifts the responsibility of infrastructure management to the cloud provider, allowing developers to focus more on writing code and delivering value.
   * Serverless computing has several key characteristics that differentiate it from traditional server-based architectures:
      * No server management: In serverless computing, developers don't have to worry about server provisioning, configuration, or management. The cloud provider abstracts away the underlying infrastructure, allowing developers to focus solely on writing code. This eliminates the operational overhead of managing servers and infrastructure.
      * Event-driven execution: Serverless computing is typically event-driven. Functions are triggered by specific events such as HTTP requests, database updates, file uploads, or scheduled timers. When an event occurs, the cloud provider automatically scales up the necessary resources and executes the corresponding function. This event-driven nature allows for more efficient resource utilization and scalability.
      * Automatic scaling: One of the key benefits of serverless computing is automatic scaling. The cloud provider dynamically allocates resources based on the incoming workload. Functions can scale up or down automatically, ensuring that they can handle varying workloads without manual intervention. This scalability allows applications to seamlessly handle traffic spikes and accommodate changing demands.
      * Pay-per-use pricing: Serverless computing follows a pay-per-use pricing model. With traditional server-based architectures, you pay for the continuous running of servers, regardless of the actual usage. In serverless, you only pay for the actual execution time and resources consumed by your functions. This cost model can provide significant cost savings, especially for applications with sporadic or unpredictable workloads.
      * Stateless and ephemeral: Serverless functions are stateless and ephemeral, meaning they do not maintain any persistent state between invocations. Each function invocation is independent and isolated. Any required state or data must be stored externally, such as in a database or storage service. This stateless nature simplifies scaling and allows for better fault tolerance and parallel execution.
      * Stateless and ephemeral: Serverless functions are stateless and ephemeral, meaning they do not maintain any persistent state between invocations. Each function invocation is independent and isolated. Any required state or data must be stored externally, such as in a database or storage service. This stateless nature simplifies scaling and allows for better fault tolerance and parallel execution.
      * Event-driven ecosystem: Serverless computing fosters an event-driven ecosystem where functions are composed together to create complex workflows or applications. Functions can be easily combined and integrated with other services or APIs, allowing developers to create serverless architectures that respond to a wide range of events and triggers.
      * Third-party service integrations: Serverless computing platforms often provide seamless integrations with various third-party services, such as databases, queues, authentication providers, and more. These integrations allow developers to leverage existing services and reduce the amount of code they need to write.
2.
   * Sign up: Visit the Vercel website at **https://vercel.com/** and sign up for an account.
   * Set up your project: Create a new directory or navigate to an existing project directory on your local machine.
   * Write your serverless function: Create a new file or directory for your serverless function and write the code for the function.
   * Configure your serverless function: Depending on the serverless platform and requirements of your function, you may need to configure certain settings or dependencies.
   * Deploy the serverless function using Vercel:

     *  **Option 1: Using Vercel CLI**
     *  Open a command prompt or terminal.
     *  Navigate to your project directory.
     *  Run the following command to deploy your function: ```vercel```
     *  **Option 2: Using Vercel web dashboard**
     *  Log in to your Vercel account and go to the Vercel web dashboard.
     *  Click on the "Import Project" button.
     *  Select your project repository or drag and drop your project directory.
     *  Configure the project settings and provide any necessary information.
     *  Click on the "Deploy" button to deploy your project.
     
   * Monitor and manage your deployed function: Once the deployment is complete, you can access and manage your deployed function from the Vercel web dashboard
   
3. API stands for Application Programming Interface. It is a set of rules and protocols that allows different software applications to communicate and interact with each other. APIs define how different components of software systems should interact, enabling developers to access and manipulate data or functionality provided by external services, libraries, or platforms.
      * Identify the API: Determine the external service or platform that provides the API you want to access. This could be a social media platform, weather service, financial data provider, or any other service that offers an API for developers to interact with.
      * Read the API documentation: APIs usually come with documentation that describes how to use them, including the available endpoints, request formats, authentication requirements, and response formats. Read the API documentation to understand the API's capabilities and how to interact with it.
      * Choose an API library: Python provides several libraries that simplify working with APIs. Popular choices include **requests**, http.client, urllib, or libraries specific to the API you're using (if available). Select the appropriate library based on your needs and the API requirements.
      * Make API requests: Use the chosen library to send HTTP requests to the API endpoints. Common request methods include GET, POST, PUT, DELETE, etc. You'll typically need to provide parameters, headers, and possibly authentication credentials as part of the request.
      * Handle the API response: Once the API responds to your request, you'll receive a response object or data. Parse and process the response according to the API's response format (e.g., JSON, XML). Extract the relevant data you need from the response and handle any errors or status codes returned by the API.
      * Manipulate the data: Once you have obtained the data from the API, you can manipulate it in your Python application as needed. This could involve performing calculations, filtering, sorting, or integrating the data with other parts of your application.



4. The **requests** library is a popular Python library for making HTTP requests and interacting with APIs. It provides a simple and intuitive interface for sending various types of HTTP requests, handling responses, and managing request sessions.
      * Install the requests library **pip install requests**
      * Import the requests module **import requests**
      * Sending a basic GET request **response = requests.get('https://api.github.com/user')**
      * Get the response status code:**print(response.status_code)**
      * Get the response content: **print(response.content)**
      * Get the response headers: **print(response.headers)**
      * Parse the response as JSON: **json_data = response.json()**
      * Iterate over the response content line by line: 
    ```python
    for line in response.iter_lines():
        print(line)
    ```



## Things I want to know more about

Serverless

Requests library 











     






     
     














