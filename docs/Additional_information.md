# SMART RF PLUS Features


## **Additional Information**

Smart RF Plus uses the  real estate of the screen to display 
additional data, enhancing the user experience and providing valuable context for warehouse operations.

### **What is it?**

Smart RF PLUS leverages the extra screen space to show additional information that can assist users in making informed decisions. This feature enhances the utility of the app by presenting relevant data alongside the primary functions.

### **Types**

- **MOCA Command**
  - Displays results or outputs from MOCA commands directly on the screen. This allows users to see real-time data and responses from the system.

  Example of using CMD to display grid

  ```sql
     [select ordnum, 
        prtnum , 
        schbat 
          from pckwrk_view 
           where wrkref = '<<FORM_ID.FIELD_ID>>'
          group by prtnum, 
          ordnum, 
          schbat 
     ] 
     |
    if (@prtnum = 'PACEMAKER')
    {
        [select count (ordlin) , 
          ordnum , 
          pckqty as ordqty , 
          schbat , 
          prtnum 
             from pckwrk_view 
              where rownum < 99 
               and schbat = **schbat 
               and appqty = '0' 
               group by ordnum,
             pckqty,
             prtnum,
            schbat
        ]
    }


- **URL**
  - Integrates web content by displaying data from specified URLs. This feature can be used to show dynamic information or web-based applications relevant to warehouse operations.

  - Example of using url to display image 
  ```sql 
       SELECT prtnum 
      FROM pckwrk_view 
          WHERE wrkref = '<<FORM_ID.FIELD_ID>>' 
      GROUP BY prtnum 
      |
      IF (**prtnum = 'YOUR ITEM')
        {
         PUBLISH DATA 
       WHERE image_url = 'https://m.media-amazon.com/images/I/    51MJdhzJ5oL._AC_.jpg' 
        }
  
   ```

- **Images**
  - Supports the display of images, which can be useful for visual references such as product photos, diagrams, or instructional images.

### **How to mantain Additional information** 
- **Form Information**
  
   To manage information displayed on forms, use the Form Information Menu. Here, you can define what additional data should appear across the screen.

  - Navigate to the form information menu  on the smart rf plus.
  - click on the add button from here  

  <div style="text-align: center;">
  <img src="./attachments/additional information/Form_info.png" 
       alt="undirectedmenu" 
       style="height: 200px; margin: auto; display: block; cursor: zoom-in; 
              border: 2px solid #000000; border-radius: 4px;" 
       onclick="this.style.height='400px'; this.style.cursor='zoom-out';" 
       ondblclick="this.style.height='200px'; this.style.cursor='zoom-in';">
  </div>



  - A new screen appears now follow the following steps: 
    - **Choose App Version** : MOCA Version which is in use
    - **Choose relevant Form ID** : Form on which you work.
    - Add **Title**, **Type**, and **Information** you want displayed.
    - You can also arrange the display order by setting a Sort Sequence, ensuring that critical data appears in the right place and in the correct order.
 
  <div style="text-align: center;">
  <img src="./attachments/additional information/Form_info_dtl.png" 
       alt="undirectedmenu" 
       style="height: 190px; margin: auto; display: block; cursor: zoom-in; 
              border: 2px solid #000000; border-radius: 4px;" 
       onclick="this.style.height='400px'; this.style.cursor='zoom-out';" 
       ondblclick="this.style.height='200px'; this.style.cursor='zoom-in';">
  </div>
  
  - Click on the save button to proceed
### 
- **Field Information**
  - The Field Information Menu lets you manage data for individual fields within a form.

  - Navigate to the form information menu  on the smart rf plus.
  - click on the add button from here 
  
  <div style="text-align: center;">
  <img src="./attachments/additional information/Field_infoi.png" 
       alt="undirectedmenu" 
       style="height: 200px; margin: auto; display: block; cursor: zoom-in; 
              border: 2px solid #000000; border-radius: 4px;" 
       onclick="this.style.height='400px'; this.style.cursor='zoom-out';" 
       ondblclick="this.style.height='200px'; this.style.cursor='zoom-in';">
  </div>

   
  - A new screen appears now follow the following steps:
    - **Choose the Field ID**:Selects on which field you want to work.
    - **Choose the App Version**: MOCA Version which is in use.
    - **Choose Form ID**: Form on which you work.
    - To link specific information to particular fields by setting the **Title**, **Type**, and **Information**, as well as the **Sort Sequence**.

  <div style="text-align: center;">
  <img src="./attachments/additional information/Form_info_dtl.png" 
       alt="undirectedmenu" 
       style="height: 200px; margin: auto; display: block; cursor: zoom-in; 
              border: 2px solid #000000; border-radius: 4px;" 
       onclick="this.style.height='400px'; this.style.cursor='zoom-out';" 
       ondblclick="this.style.height='200px'; this.style.cursor='zoom-in';">
  </div>
  
  - Click on the Save button to proceed


- **Additional Information Via Remote Server**
  - Commands can be securely stored in your server within the **Les CMD** table.
  - Ensure that the **Command ID** is referenced in the **Additional Information** section under **Smart-Apps Field/Form Info**.
  
  <div style="text-align: center;">
  <img src="./attachments/additional information/Additionalinforemoteserver.png" 
       alt="undirectedmenu" 
       style="height: 200px; width:450px; margin: auto; display: block; cursor: zoom-in; 
              border: 2px solid #000000; border-radius: 4px;" 
       onclick="this.style.height='400px'; this.style.cursor='zoom-out';" 
       ondblclick="this.style.height='200px'; this.style.cursor='zoom-in';">
  </div>

  - Commands are executed through the **MOCA Server** and should be properly referenced in the Info section, as shown in the image above.
  - **Remote command Flag** is **Enabled** as shown in the image above.







