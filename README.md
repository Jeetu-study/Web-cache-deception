# Web-cache-deception

***simple story hai cache hit aya response main to matlb hua ki jo response aya hai vo cache se hit hoke aya hai </br>but agar response main aya cache-miss to response origanal server se aya hai kyuki cache hit nhi ho paya miss ho gaya***</br></br>

***ab application main kahi baar hota ye hai ki kuch response cache server se ata hai but kuch response always orignal server se hi ate hai***
</br></br></br>

***To yaha per ye vulnerbulity hai ki humko vo end point dekhna hai jiska response chache server se aa raha hai or us server per humko ek cache file name create krna hai. or us usrl ko orignal url ke sath bind krke victim ko dena hai</br></br></br> isse hoga ye ki jo victim for example koi senstive page ko dekh raha hai jaha per uske account ki info details hai jab attacker ka banaye hua link victim click krega tab vo url bhi cache main chala jayega vo url phele orignal server se hi response de raha tha but ye single time hoga and attacker ke pass victim ki senstive info cache server se aa jayegi***</br></br></br>


<img width="960" alt="image" src="https://github.com/user-attachments/assets/e409635a-98a3-43b0-9374-2f4f30e3a2ce">
</br></br>

***Yaha poc main attacker ne abc.js file name diya jo phele tracking.js tha and is url ko orignal url ke sath bind kr diya***</br></br>

<img width="960" alt="image" src="https://github.com/user-attachments/assets/2a1eb1a9-e3ad-41ac-8a64-267a0cdc6bfb">

</br></br>

***ye phele myaccount tk tha url per attacker ne resources/js/abc.js ye path ko cahch krwa diya hai or ye pata bana kr https://0ab900e203e2a024808e12d80022008c.web-security-academy.net/my-account/resources/js/abc.js victim ko send kiya body ke under </br></br> <script>document.location="https://0ab900e203e2a024808e12d80022008c.web-security-academy.net/my-account/resources/js/abc.js"</script></br></br> daal kr csrf poc share ki or jaise victim is link per click kra uski senstive info attacker ke pass aa gayi***</br></br>

<img width="959" alt="image" src="https://github.com/user-attachments/assets/193b7a28-2827-46a8-ac40-f81846fd3ef8">







