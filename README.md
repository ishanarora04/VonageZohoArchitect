# VonageZohoArchitect

### This is an architectural diagram for a solution which uses ZohoOne, Vonage and a custom Webapp for this purpose

<div align="center">
    <img src="/vonageZoho.png" width="700px"</img> 
</div>

<p> 
    A proposed solution relies on using zoho one , webapp and vonage for achieving the desired business impact.
    1.  If the lead is not created in the business hours, no broadcast call to all sales representative will be made.A lead will be directly created in Zoho via the the webapp.
    </br>
    2.  If the lead is created in the business hours , we will follow the approach as shown in the screenshot above. When a webhook is received from a call representative , we will update the status of lead in Zoho to assigned. Any further webhooks will check this status and be rejected. We will disconnect those calls. 
   </br>
    3.  We will heavily rely on conversational API of Vonage which connects the caller and the callee from an end. 
    </br>
    4.  We expect the sales representatives already have a Vonage Client SDK based functionality with him. It can be in the form of mobile application, Web UI or directly integrated with Zoho One. 
    
<p/>
