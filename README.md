# FreePBX_CID-to-Monica
This approach allows you to include the calling number ($thenumber) dynamically in the content field of your API request to Monica CRM. Adjust the content message and any other fields as needed based on your application's requirements and Monica CRM API specifications.

<< Requirement >>
   FreePBX,
   Monica CRM,
   Monica Bearer authentication
   

<< INSTALL >>
   In the FreePBX GUI Go to <ADMIN/CID Superfecta> under name click "Defalt" look for Send to URL and Enable it. 
    In FreePBX CLI Command or Filezilla edit < /var/www/html/admin/modules/superfecta/sources/source-Send_to_URL.module > Copy past code in [source-Send_to_URL.module](https://github.com/basskillin/CID-to-Monica_FreePBX/blob/main/source-Send_to_URL.module). Edit 'default' => "YOUR_API_LINK_HERE",  'default' => 'YOUR_BEARER_TOKEN_HERE', and  'contact_id' => 3,   // Specific contact_id as required. Pick a contact in Monica to Use.  If all went well it should work. 
