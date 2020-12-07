## Complete backend and database under 15 minutes for any application! (React / Angular / Vue) AWS Amplify Admin UI 🔥 - Getting started

# What? 🤔

- AWS recently released Amplify Admin UI, which enables you to seamlessly create back-end and cloud databases for your next project!
- Supported for: web, android, iOS
- Support for Android: Java, Kotlin
- Support for iOS: SwiftUI
- Frameworks support for web: React, Angular, Vue

# How? 💭

- Install the node package manager
- Install AWS amplify CLI as:
```
npm install -g @aws-amplify/cli
```

- Head over to [Amplify Admin](https://sandbox.amplifyapp.com/getting-started)
![Capture.PNG](https://cdn.hashnode.com/res/hashnode/image/upload/v1607227356067/FuAex0eC4.png)
- And click "Get started"

![Capture.PNG](https://cdn.hashnode.com/res/hashnode/image/upload/v1607227461923/BSf_1zZbF.png)
- You will see something like the above picture, now if you don't have an AWS account you can try this out by selecting "Data" and a local sandbox will be created for you.

- After selecting data, you will be asked to select a scheme, for this post I will go with "blank schema" because we want to create our own. 

#### Now let's add a model. Amplify follows a NoSQL DB. So, here the model is relatable to a table in SQL

![Capture.PNG](https://cdn.hashnode.com/res/hashnode/image/upload/v1607227896724/5F4QW7NcD.png)

- After adding a model, you can create its fields, as I did:

![Capture.PNG](https://cdn.hashnode.com/res/hashnode/image/upload/v1607227976673/elkgry50U.png)

#### Now we'll go for testing this model in our application, to proceed further select the button in the top right corner, which says "Next: Test locally in your app"
![Capture.PNG](https://cdn.hashnode.com/res/hashnode/image/upload/v1607228584885/dbVVF4BJz.png)

### Testing

- You can select any of the supported platform and framework you like, for this post I will be selecting Web as the platform and React as a framework.
- After selecting the platform and the framework. Click next and follow the step mentioned there.
- Now as you have AWS amplify installed, and your application setup, it's time for pulling the amplify sandbox configurations into your application.
```
amplify pull --sandboxId your-sandbox-id-here-without-quotation-marks
```
- Now, install aws-amplify and typescript library to your react application.
```
npm install aws-amplify typescript
```
- Use the following code in index.js, to configure your application

```
import Amplify from 'aws-amplify'
import awsconfig from './aws-exports'

Amplify.configure(awsconfig);
```
- Now we are ready to test ours react application with AWS Amplify.
![Capture.PNG](https://cdn.hashnode.com/res/hashnode/image/upload/v1607229255278/GIv_BAZOu.png)
#### You can play around and test the various CRUD operations locally to see how it all works and later you can deploy it to the cloud ( need an AWS account for this ).

### That's all for this blog post, will see you in the next post, with another awesome and useful resources to share with the community. 😄

- Feel free to connect with me on Twitter @ [amaancodes](https://twitter.com/amaancodes)