Issues

When going to "Frontend environments" to associate a GitHub repo.
Only works in Chrome, Brave and Safari advise to delete cookies, even with no prior Safari login.
https://us-east-1.console.aws.amazon.com/amplify/home?region=us-east-1#/

Instead, try these [steps](https://aws.amazon.com/getting-started/hands-on/build-react-app-amplify-graphql/module-one/?e=gs2020&p=build-a-react-app-intro) to associate to GitHub before adding Amplify.  

I did the Github checkout first using GitHub Desktop (step 2 before step 1), otherwise

	git commit -m “initial commit”

Returns error:
error: pathspec ‘commit”’ did not match any file(s) known to git

---

Blue "Deploy" image needs to be replaced with white "Deliver" image.
https://aws.amazon.com/getting-started/hands-on/build-react-app-amplify-graphql/module-one/?e=gs2020&p=build-a-react-app-intro

---

amplifyapp % git commit -m “changes for v2”
error: pathspec 'for' did not match any file(s) known to git
error: pathspec 'v2”' did not match any file(s) known to git

Use ticks instead (for Mac, test on PC):

	git commit -m 'changes for v2'

---

Used Github Desktop instead due to error from:

	git push origin master

error: src refspec master does not match any
error: failed to push some refs to 'https://github.com/modelearth/amplifyapp.git'

Try renaming to "main"

git commit -m 'test commit'

---

Code box for GitHub commands says "Javascript", should just say "Script" or "Commands"

https://aws.amazon.com/getting-started/hands-on/build-react-app-amplify-graphql/module-one/?e=gs2020&p=build-a-react-app-intro

---