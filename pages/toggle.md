---
title: Toggle Parts of Layouts
description: How to toggle parts of layouts on user input.
published: true
date: 2024-02-26T09:56:51.707Z
tags: 
editor: markdown
dateCreated: 2024-02-26T05:08:33.154Z
---

# Toggle Parts of Layouts

Sometimes it's good to have the choice! Maybe some of your users don't like constantly hearing Rick Astley as menu music or want a different cute anime girl as menu background.

Well, that's no problem! You can make it so your users can toggle on/off parts of your layouts or cycle through multiple versions of said parts.

# Toggle On/Off

To toggle, for example, the visibility of an element by clicking a button, you just need to use a variable that gets set on button click and the element you want to toggle needs to check in its loading requirements if said variable has the correct value.

## The Variable

The first thing is creating the variable you will use to store the visibility state of the element you want to toggle.

To add a new variable, navigate to the **Customization** tab in the menu bar and click on **Variables -> Manage Variables**, then add a new variable with a **unique** name! Make sure to use a really **unique** name that isn't used already.

After creating the variable, set its value to `true`.

<br>
<img width="494" alt="Screenshot_9" src="https://gist.github.com/assets/35544624/1e29be13-e601-4669-8fa2-d78db945b07f">

## The Element

The next step is to add the element you want to toggle on/off.

<br>
<img width="270" alt="Screenshot_3" src="https://gist.github.com/assets/35544624/317460fc-310b-4941-ab9a-b56490c5ebb9">

Now right-click the element and click on **Loading Requirements**.
This will open the Manage Requirements screen. Click on **Add Requirement**.

Search for the **Is Variable Value** requirement, select it and click on **Edit Requirement Value**.

<br>
<img width="501" alt="Screenshot_1" src="https://gist.github.com/assets/35544624/d0d342f5-617c-415e-b6f7-05087fc204b7">

Now input the name of the variable you created earlier and let the requirement check for `true` as value.

<br>
<img width="500" alt="Screenshot_2" src="https://gist.github.com/assets/35544624/a1f356e9-7f96-4d8b-87b0-51f05898409a">

That's it for that part. Now your element will be visible when the variable's value is `true`.

## The Button

Now we need to add a new Button element.

<br>
<img width="270" alt="Screenshot_4" src="https://gist.github.com/assets/35544624/1bd1b781-0cdb-4b52-80a0-db8f44ead0db">

After adding, right-click it and click on **Edit Action Script**.
This will open the button's Manage Action Script screen.

Click on **Add IF Statement**, add the **Is Variable Value** requirement to it and set the requirement's mode to **OPPOSITE**.

<br>
<img width="520" alt="Screenshot_5" src="https://gist.github.com/assets/35544624/a024ea21-2244-4ca6-b44b-1a80f7936b8f">

Now click on **Edit Requirement Value**, just like you did with the element before and just input the exact same variable name and value to check for.

<br>
<img width="500" alt="Screenshot_2" src="https://gist.github.com/assets/35544624/a1f356e9-7f96-4d8b-87b0-51f05898409a">

Because we set the requirement mode to **OPPOSITE**, it will now check if the variable value is NOT `true`, which is exactly what we want.

Back in the Edit Action Script screen you will now see the IF statement we just added.

<br>
<img width="495" alt="Screenshot_6" src="https://gist.github.com/assets/35544624/6ac8444c-ca15-43ff-a633-df63e76e7433">

Now click on **Add Action**, search for the **Set Variable Value** action, select it and then click on **Edit Action Value**.

<br>
<img width="494" alt="Screenshot_7" src="https://gist.github.com/assets/35544624/8568e539-b4d0-49bd-89c4-4659ee71754c">

As action value, input your variable name first and the value you want to set it to after. Separate name and value by `:`.
In this case we want to set our value to `true`, because this action later gets executed when the value is NOT `true`.

<br>
<img width="496" alt="Screenshot_8" src="https://gist.github.com/assets/35544624/fab440ad-b335-4751-9651-4bb0b65bc968">

Now append the action to the IF statement by grabbing and moving it over the IF statement, so it only gets executed when our variable's value is NOT `true`.

<br>
<img width="496" alt="Screenshot_8" src="https://gist.github.com/assets/35544624/d1ac3ea9-44d7-4ad6-a4b2-455b21f6d1c4">

After doing that, select the IF statement and then click on **Append ELSE Statement**.

Now add another **Set Variable Value** action, but instead of setting the variable value to `true`, set it to `false`.

<br>
<img width="494" alt="Screenshot_9" src="https://gist.github.com/assets/35544624/d05400dc-b9b7-4c1a-8657-9e34939ed599">

Now append the second action to the ELSE statement, so it gets executed if the variable value IS `true`.

<br>
<img width="494" alt="Screenshot_9" src="https://gist.github.com/assets/35544624/3191a1cc-c5c2-4cf1-a620-23bdbe639bf2">

And that's it! Feels like lots of steps the first time, but it's actually a pretty easy and quick thing to do once you got used to it.

Now you can save your layout, leave the editor and press the button to see if it works!

<br>
<img width="494" alt="Screenshot_9" src="https://gist.github.com/assets/35544624/e9a87aca-ba0f-4ce6-a39e-1e1d3796c9e3">

Feel free to use the same variable for other elements, so you **toggle multiple elements at once** by pressing the button.

You can even toggle whole layouts by using the **Layout-Wide Loading Requirements**. To configure layout-wide requirements, right-click the editor background. Just make sure to add the button to another layout, not the one you want to toggle.

# Cycle Through

Other than toggling between two values, cycling through values needs the action script to be able to cycle between more than two values.

The action script logic is really similar to the one used for toggling, so I will keep it really short here. Make sure to also read the part about toggling.

I added 3 images. The first image is visible when the variable value is `1`, the second one if the value is `2` and the third one if the value is `3`.

<br>
<img width="494" alt="Screenshot_9" src="https://gist.github.com/assets/35544624/731c13cf-6f81-470b-8e1b-cba264ffbe05">

After that I added the cycle button and made it cycle the variable value from `1` to `2` to `3` to `1`.

<br>
<img width="609" alt="Screenshot_1" src="https://gist.github.com/assets/35544624/9f2052b1-8d3d-4a35-884a-4a234e63d5e5">

And that's it. Now save the layout, leave the editor and check if the cycle button is working correctly.

<br>
<img width="494" alt="Screenshot_9" src="https://gist.github.com/assets/35544624/430c2369-a43f-4d0f-9203-3fdb1b9eae2c">
