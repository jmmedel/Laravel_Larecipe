

Vue Components Support
Because LaRecipe renders the documentations in the back-end of Laravel application, it's pretty cool to leverage custom VueJs components.

Cards
Buttons
Badges
Progress
Built-in Components
LaRecipe provides a bunch of amazing looking UI Vue based components. Thanks to Argon again!

If you don't like the idea of mixing Vue components with Markdown, remember that this feature is optional.


Cards
Input:

<larecipe-card>
    Example card
</larecipe-card>
Output:

Example card

Buttons
Input:

<larecipe-button>
    Example button
</larecipe-button>
Output:


Badges
Input:

<larecipe-badge type="primary" circle icon="fa fa-user"></larecipe-badge>
<larecipe-badge type="success">Holly</larecipe-badge>
<larecipe-badge type="danger">Molly</larecipe-badge>
Output:

 HOLLA MOLLY

Progress
Input:

<larecipe-progress type="success" :value="60"></larecipe-progress>
Output:

60%
You can achieve the same effect on the installation page by including a progress component inside a card.

Input:

<larecipe-card>
    <larecipe-badge type="success" circle class="mr-3" icon="fa fa-heart"></larecipe-badge> BinaryTorch
    <larecipe-progress type="success" :value="100"></larecipe-progress>
</larecipe-card>
Output:
