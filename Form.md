## Functions

<dl>
<dt><a href="#initFormAsync">initFormAsync(callback)</a></dt>
<dd><p>Initializes and returns an empty form object based on the default form file present in the package</p>
</dd>
<dt><a href="#submitFormRequest">submitFormRequest(form)</a></dt>
<dd><p>Submits the newly created form as a request. This results a new conversation card</p>
</dd>
<dt><a href="#submitFormRequestV2">submitFormRequestV2(form)</a></dt>
<dd><p>Submits the newly created form as a request. This results a new conversation card</p>
</dd>
<dt><a href="#submitFormRequestWithResponses">submitFormRequestWithResponses(form)</a></dt>
<dd><p>Submits the newly created form as a request with responses</p>
</dd>
<dt><a href="#submitFormRequestWithoutDismiss">submitFormRequestWithoutDismiss(form)</a></dt>
<dd><p>Submits the newly created form as a request. This results a new conversation card</p>
</dd>
<dt><a href="#updateForm">updateForm()</a></dt>
<dd><p>use for making changes in form fields like title, description and settings.</p>
</dd>
<dt><a href="#canRespondToFormAsync">canRespondToFormAsync(callback)</a></dt>
<dd><p>Gets whether the current user can respond to the form</p>
</dd>
<dt><a href="#getFormAsync">getFormAsync(callback)</a></dt>
<dd><p>Gets the form object associated with the conversation card</p>
</dd>
<dt><a href="#getFormStatusAsync">getFormStatusAsync(callback)</a></dt>
<dd><p>Gets the status of the form associated with the conversation card</p>
</dd>
<dt><a href="#getMyFormResponsesAsync">getMyFormResponsesAsync(callback)</a></dt>
<dd><p>Gets all the responses of the current user against the form</p>
</dd>
<dt><a href="#getBatchResponsesAsync">getBatchResponsesAsync(callback)</a></dt>
<dd><p>Gets all the responses of the current user against the form</p>
</dd>
<dt><a href="#getResponsesForTimeRangeAsync">getResponsesForTimeRangeAsync(startTime, endTime, userId, callback)</a></dt>
<dd><p>Gets all the responses of the current form for given time range</p>
</dd>
<dt><a href="#sumbitFormResponse">sumbitFormResponse(questionToAnswerMap, responseId, isEdit, showInChatCanvas, isAnonymous)</a></dt>
<dd><p>Submits a new response against the form associated with the conversation card
This will dismiss the current screen</p>
</dd>
<dt><a href="#sumbitFormResponseWithoutDismiss">sumbitFormResponseWithoutDismiss(questionToAnswerMap, responseId, isEdit, showInChatCanvas, isAnonymous)</a></dt>
<dd><p>Submits a new response against the form associated with the conversation card
This won&#39;t dismiss the current screen</p>
</dd>
<dt><a href="#sumbitBatchFormResponse">sumbitBatchFormResponse(responses, showInChatCanvas, isAnonymous, shouldDismis)</a></dt>
<dd><p>Submits a new response against the form associated with the conversation card
This won&#39;t dismiss the current screen</p>
</dd>
<dt><a href="#shouldSeeFormSummaryAsync">shouldSeeFormSummaryAsync(callback)</a></dt>
<dd><p>Gets whether the form summary is visible to the current user</p>
</dd>
<dt><a href="#getFormUserCapabilitiesAsync">getFormUserCapabilitiesAsync(callback)</a></dt>
<dd><p>Gets form permissions</p>
</dd>
<dt><a href="#isSubscribed">isSubscribed(callback)</a></dt>
<dd><p>Gets whether the current user is subscriber or not</p>
</dd>
<dt><a href="#getFormSummaryAsync">getFormSummaryAsync(mostUpdatedCallback, notifyCallback)</a></dt>
<dd><p>Gets flat responses by all the users, and processed summary from all the responses associated
with the form. It requires two callbacks:</p>
</dd>
<dt><a href="#getFlatFormSummaryAsync">getFlatFormSummaryAsync(callback)</a></dt>
<dd><p>Gets flat responses by all the users associated with the form (It is advised to use getFormSummary() instead of this)</p>
</dd>
<dt><a href="#getProcessedFormSummaryAsync">getProcessedFormSummaryAsync(callback)</a></dt>
<dd><p>Gets processed summary from all the responses associated with the form (It is advised to use getFormSummary() instead of this)</p>
</dd>
<dt><a href="#getAggregatedFormSummaryAsync">getAggregatedFormSummaryAsync(callback)</a></dt>
<dd><p>Gets aggregated summary from all the responses associated with the form</p>
</dd>
<dt><a href="#getFormURLAsync">getFormURLAsync(callback)</a></dt>
<dd><p>Gets the file url from server containing flat responses associated with the form</p>
</dd>
<dt><a href="#shareFormURL">shareFormURL(url)</a></dt>
<dd><p>Launches native share screen for the form url</p>
</dd>
<dt><a href="#getFormReactionAsync">getFormReactionAsync(callback)</a></dt>
<dd><p>Gets the consolidated reaction (likes and comments) of the conversation card associated with the form</p>
</dd>
<dt><a href="#showAllReactions">showAllReactions()</a></dt>
<dd><p>Shows all the reaction screen (likes and comments) against the form</p>
</dd>
<dt><a href="#likeForm">likeForm()</a></dt>
<dd><p>Requests to add a like count to a form, the count may decrease if the current user has already liked the form</p>
</dd>
<dt><a href="#addCommentOnForm">addCommentOnForm()</a></dt>
<dd><p>Requests to add a comment to a form</p>
</dd>
<dt><a href="#respondToForm">respondToForm()</a></dt>
<dd><p>Requests to add a response to a form, by launching response screen</p>
</dd>
<dt><a href="#sendRemindersToRespond">sendRemindersToRespond()</a></dt>
<dd><p>Sends a reminder (a new conversation card) against the existing card</p>
</dd>
<dt><a href="#copyFormAndForward">copyFormAndForward()</a></dt>
<dd><p>Launches the conversation picker to forward a copy of the existing form as a new conversation card</p>
</dd>
<dt><a href="#closeForm">closeForm()</a></dt>
<dd><p>Closes the form associated with the card, no responses will be allowed further</p>
</dd>
<dt><a href="#showEditFormPage">showEditFormPage()</a></dt>
<dd><p>Editing the form associated with the card.</p>
</dd>
<dt><a href="#updateFormPropertiesAsync">updateFormPropertiesAsync(propertyUpdates, notifyUsers, notificationMessage, callback)</a></dt>
<dd><p>Post a request to update the properties associated with the form</p>
</dd>
<dt><a href="#sendNotificationToUsers">sendNotificationToUsers(customNotificationMessage, callback)</a></dt>
<dd><p>Requests to send push notification to a particular set of users with a custom message</p>
</dd>
</dl>

<a name="initFormAsync"></a>

## initFormAsync(callback)
Initializes and returns an empty form object based on the default form file present in the package

**Kind**: global function  

| Param | Type | Description |
| --- | --- | --- |
| callback | <code>Callback</code> | with below parameters: * * * @param {KASForm} form can be null in case of error * * * @param {string} error message in case of error, null otherwise |

<a name="submitFormRequest"></a>

## submitFormRequest(form)
Submits the newly created form as a request. This results a new conversation card

**Kind**: global function  

| Param | Type |
| --- | --- |
| form | <code>KASForm</code> | 

<a name="submitFormRequestV2"></a>

## submitFormRequestV2(form)
Submits the newly created form as a request. This results a new conversation card

**Kind**: global function  

| Param | Type |
| --- | --- |
| form | <code>KASForm</code> | 

<a name="submitFormRequestWithResponses"></a>

## submitFormRequestWithResponses(form)
Submits the newly created form as a request with responses

**Kind**: global function  

| Param | Type |
| --- | --- |
| form | <code>KASForm</code> | 

<a name="submitFormRequestWithoutDismiss"></a>

## submitFormRequestWithoutDismiss(form)
Submits the newly created form as a request. This results a new conversation card

**Kind**: global function  

| Param | Type |
| --- | --- |
| form | <code>KASForm</code> | 

<a name="updateForm"></a>

## updateForm()
use for making changes in form fields like title, description and settings.

**Kind**: global function  
<a name="canRespondToFormAsync"></a>

## canRespondToFormAsync(callback)
Gets whether the current user can respond to the form

**Kind**: global function  

| Param | Type | Description |
| --- | --- | --- |
| callback | <code>Callback</code> | with below parameters: * * * @param {boolean} canRespond true if current user is allowed to respond |

<a name="getFormAsync"></a>

## getFormAsync(callback)
Gets the form object associated with the conversation card

**Kind**: global function  

| Param | Type | Description |
| --- | --- | --- |
| callback | <code>Callback</code> | with below parameters: * * * @param {KASForm} form can be null in case of error * * * @param {string} error message in case of error, null otherwise |

<a name="getFormStatusAsync"></a>

## getFormStatusAsync(callback)
Gets the status of the form associated with the conversation card

**Kind**: global function  

| Param | Type | Description |
| --- | --- | --- |
| callback | <code>Callback</code> | with below parameters: * * * @param {boolean} isActive true if the form is not yet expired * * * @param {string} error message in case of error, null otherwise |

<a name="getMyFormResponsesAsync"></a>

## getMyFormResponsesAsync(callback)
Gets all the responses of the current user against the form

**Kind**: global function  

| Param | Type | Description |
| --- | --- | --- |
| callback | <code>Callback</code> | with below parameters: * * * @param {KASFormResponse[]} responses can be null in case of error * * * @param {string} error message in case of error, null otherwise |

<a name="getBatchResponsesAsync"></a>

## getBatchResponsesAsync(callback)
Gets all the responses of the current user against the form

**Kind**: global function  

| Param | Type | Description |
| --- | --- | --- |
| callback | <code>Callback</code> | with below parameters: * * * @param {KASFormResponse[]} responses can be null in case of error * * * @param {string} error message in case of error, null otherwise |

<a name="getResponsesForTimeRangeAsync"></a>

## getResponsesForTimeRangeAsync(startTime, endTime, userId, callback)
Gets all the responses of the current form for given time range

**Kind**: global function  

| Param | Type | Description |
| --- | --- | --- |
| startTime | <code>number</code> | start timestamp of time range |
| endTime | <code>number</code> | end timestamp of time range |
| userId | <code>string</code> | for which response will be fetched. Should be empty to fetch responses of whole survey. |
| callback | <code>Callback</code> | with below parameters: * * * @param {KASFormResponse[]} responses of the survey for given userId. |

<a name="sumbitFormResponse"></a>

## sumbitFormResponse(questionToAnswerMap, responseId, isEdit, showInChatCanvas, isAnonymous)
Submits a new response against the form associated with the conversation cardThis will dismiss the current screen

**Kind**: global function  

| Param | Type | Description |
| --- | --- | --- |
| questionToAnswerMap | <code>JSON</code> | question id to answer mapping |
| responseId | <code>string</code> | to be filled if the current response is an edit/update to a previous one |
| isEdit | <code>boolean</code> | denotes if the current response is an edit/update to a previous one |
| showInChatCanvas | <code>boolean</code> | denotes if a separate chat card needs to be created for this response or not |
| isAnonymous | <code>boolean</code> | denotes if the response should be registered as anonymous or not |

<a name="sumbitFormResponseWithoutDismiss"></a>

## sumbitFormResponseWithoutDismiss(questionToAnswerMap, responseId, isEdit, showInChatCanvas, isAnonymous)
Submits a new response against the form associated with the conversation cardThis won't dismiss the current screen

**Kind**: global function  

| Param | Type | Description |
| --- | --- | --- |
| questionToAnswerMap | <code>JSON</code> | question id to answer mapping |
| responseId | <code>string</code> | to be filled if the current response is an edit/update to a previous one |
| isEdit | <code>boolean</code> | denotes if the current response is an edit/update to a previous one |
| showInChatCanvas | <code>boolean</code> | denotes if a separate chat card needs to be created for this response or not |
| isAnonymous | <code>boolean</code> | denotes if the response should be registered as anonymous or not |

<a name="sumbitBatchFormResponse"></a>

## sumbitBatchFormResponse(responses, showInChatCanvas, isAnonymous, shouldDismis)
Submits a new response against the form associated with the conversation cardThis won't dismiss the current screen

**Kind**: global function  

| Param | Type | Description |
| --- | --- | --- |
| responses | <code>Array.&lt;KASFormBatchResponseUnit&gt;</code> | question id to answer mapping |
| showInChatCanvas | <code>boolean</code> | denotes if a separate chat card needs to be created for this response or not |
| isAnonymous | <code>boolean</code> | denotes if the response should be registered as anonymous or not |
| shouldDismis | <code>boolean</code> | denotes the current screen will dismiss or not |

<a name="shouldSeeFormSummaryAsync"></a>

## shouldSeeFormSummaryAsync(callback)
Gets whether the form summary is visible to the current user

**Kind**: global function  

| Param | Type | Description |
| --- | --- | --- |
| callback | <code>Callback</code> | with below parameters: * * * @param {boolean} shouldSeeSummary true if current user is allowed to see summary |

<a name="getFormUserCapabilitiesAsync"></a>

## getFormUserCapabilitiesAsync(callback)
Gets form permissions

**Kind**: global function  

| Param | Type | Description |
| --- | --- | --- |
| callback | <code>Callback</code> | with below parameters: * * * @param {KASFormUserCapabilities} permissions |

<a name="isSubscribed"></a>

## isSubscribed(callback)
Gets whether the current user is subscriber or not

**Kind**: global function  

| Param | Type | Description |
| --- | --- | --- |
| callback | <code>Callback</code> | with below parameters: * * * @param {boolean} isSubscribed true if current user subscriber |

<a name="getFormSummaryAsync"></a>

## getFormSummaryAsync(mostUpdatedCallback, notifyCallback)
Gets flat responses by all the users, and processed summary from all the responses associatedwith the form. It requires two callbacks:

**Kind**: global function  

| Param | Type | Description |
| --- | --- | --- |
| mostUpdatedCallback | <code>Callback</code> | to immediately get the most updated summary from local database. It has below parameters: * * * @param {KASFormFlatSummary} flatSummary can be null in case of error * * * @param {KASFormProcessedSummary} processedSummary can be null in case of error * * * @param {string} error message in case of error, null otherwise |
| notifyCallback | <code>Callback</code> | to get notified with the latest summary fetched from server. It has below parameters: * * * @param {KASFormFlatSummary} flatSummary can be null in case of error * * * @param {KASFormProcessedSummary} processedSummary can be null in case of error * * * @param {string} error message in case of error, null otherwise This is useful when the network is flaky/disconnected, so that summary can immediately be shown with the present data we have, but with an option to refresh it later on arrival of latest data from server! None of the callbacks are mandatory, so if 1st is nil, this method can be used to always fetch summary from server, and if 2nd is nil, this can be used to always fetch summary from local database! |

<a name="getFlatFormSummaryAsync"></a>

## getFlatFormSummaryAsync(callback)
Gets flat responses by all the users associated with the form (It is advised to use getFormSummary() instead of this)

**Kind**: global function  

| Param | Type | Description |
| --- | --- | --- |
| callback | <code>Callback</code> | with below parameters: * * * @param {KASFormFlatSummary} flatSummary can be null in case of error * * * @param {string} error message in case of error, null otherwise |

<a name="getProcessedFormSummaryAsync"></a>

## getProcessedFormSummaryAsync(callback)
Gets processed summary from all the responses associated with the form (It is advised to use getFormSummary() instead of this)

**Kind**: global function  

| Param | Type | Description |
| --- | --- | --- |
| callback | <code>Callback</code> | with below parameters: * * * @param {KASFormProcessedSummary} processedSummary can be null in case of error * * * @param {string} error message in case of error, null otherwise |

<a name="getAggregatedFormSummaryAsync"></a>

## getAggregatedFormSummaryAsync(callback)
Gets aggregated summary from all the responses associated with the form

**Kind**: global function  

| Param | Type | Description |
| --- | --- | --- |
| callback | <code>Callback</code> | with below parameters: * * * @param {KASFormAggregatedSummary} aggregatedSummary can be null in case of error * * * @param {string} error message in case of error, null otherwise |

<a name="getFormURLAsync"></a>

## getFormURLAsync(callback)
Gets the file url from server containing flat responses associated with the form

**Kind**: global function  

| Param | Type | Description |
| --- | --- | --- |
| callback | <code>Callback</code> | with below parameters: * * * @param {string} url can be null in case of error * * * @param {string} error message in case of error, null otherwise |

<a name="shareFormURL"></a>

## shareFormURL(url)
Launches native share screen for the form url

**Kind**: global function  

| Param | Type | Description |
| --- | --- | --- |
| url | <code>string</code> | to be shared |

<a name="getFormReactionAsync"></a>

## getFormReactionAsync(callback)
Gets the consolidated reaction (likes and comments) of the conversation card associated with the form

**Kind**: global function  

| Param | Type | Description |
| --- | --- | --- |
| callback | <code>Callback</code> | with below parameters: * * * @param {KASFormReaction} reaction can be null in case of error * * * @param {string} error message in case of error, null otherwise |

<a name="showAllReactions"></a>

## showAllReactions()
Shows all the reaction screen (likes and comments) against the form

**Kind**: global function  
<a name="likeForm"></a>

## likeForm()
Requests to add a like count to a form, the count may decrease if the current user has already liked the form

**Kind**: global function  
<a name="addCommentOnForm"></a>

## addCommentOnForm()
Requests to add a comment to a form

**Kind**: global function  
<a name="respondToForm"></a>

## respondToForm()
Requests to add a response to a form, by launching response screen

**Kind**: global function  
<a name="sendRemindersToRespond"></a>

## sendRemindersToRespond()
Sends a reminder (a new conversation card) against the existing card

**Kind**: global function  
<a name="copyFormAndForward"></a>

## copyFormAndForward()
Launches the conversation picker to forward a copy of the existing form as a new conversation card

**Kind**: global function  
<a name="closeForm"></a>

## closeForm()
Closes the form associated with the card, no responses will be allowed further

**Kind**: global function  
<a name="showEditFormPage"></a>

## showEditFormPage()
Editing the form associated with the card.

**Kind**: global function  
<a name="updateFormPropertiesAsync"></a>

## updateFormPropertiesAsync(propertyUpdates, notifyUsers, notificationMessage, callback)
Post a request to update the properties associated with the form

**Kind**: global function  

| Param | Type | Description |
| --- | --- | --- |
| propertyUpdates | <code>Array.&lt;KASFormPropertyUpdateInfo&gt;</code> | an array of all update infos that are needed to be performed, update infos can be created using KASFormPropertyUpdateFactory |
| notifyUsers | <code>Array.&lt;string&gt;</code> | send push notifications to these user ids regarding this update |
| notificationMessage | <code>string</code> | push notification message |
| callback | <code>Callback</code> | with below parameters: * * * @param {boolean} success indicates if the update is successful or not |

<a name="sendNotificationToUsers"></a>

## sendNotificationToUsers(customNotificationMessage, callback)
Requests to send push notification to a particular set of users with a custom message

**Kind**: global function  

| Param | Type | Description |
| --- | --- | --- |
| customNotificationMessage | <code>CustomNotificationMessage</code> | list of userIds to whom the notification has to be sent |
| callback | <code>Callback</code> | with below parameters: * * * @param {boolean} success indicates if the update is successful or not * * * @param {string} error message in case of error, null otherwise |

