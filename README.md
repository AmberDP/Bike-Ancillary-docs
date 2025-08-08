# Bike Ancillary - Documentation Overview 
Welcome to this overview page where you can find all the links to the documents needed for the integration of our API.

<img src="https://storage.googleapis.com/qover-assets/guidelines/Logo/logo-qover.svg" alt="drawing" width="200"/>

## 1. Frontend guide
[This guide](https://drive.google.com/file/d/1Jws1vasDoXREzpCRNbF7g4bcR-NR2EdB/view?usp=sharing) gives you some more context when planning your integration and gives guidance on the frontend implementations that need to be done. 

### a. Auto-generated product page ###
In the Frontend documentation you will find some explanation on how to build a product page. A **product page** is a **standalone website page** entirely dedicated to the insurance product, it summarizes the product and serves as a FAQ for your customers. It is a **legal requirement** and it is **mandatory** to have this page per country and language. As this product page can be a pain to integrate, we developed **3 ways to easily integrate an auto-generated product page by Qover on your website**. You can find it [here](https://jsfiddle.net/harryqover/bx5go9fq/latest) in jsfiddle.

## 2. Flow diagram
Start with our [flow diagram](https://drive.google.com/file/d/1TQQvkcbywUfiTB0q_S9hWI2YJQkGfPK0/view?usp=sharing) to understand how you have to integrate our API.
![BIKE Schema Ancillary API_20220214](https://user-images.githubusercontent.com/99665011/154225608-74b5c6e2-c993-4778-a665-59b853ea1bfa.png)

## 3. Financial flow
Here you can find an example of how the [financial flow](https://drive.google.com/file/d/18heqN0fItB3aWGxlLOC0XzuPPWQjN2SU/view?usp=sharing) will look like.
![Financial_flow drawio](https://user-images.githubusercontent.com/99665011/154225476-c84e7beb-9217-43be-9e2b-a8e27a175459.png)

(!) No **VAT** should be accounted for the bike insurance product. 

```Note: the insurance tax is already included in the insurance premium paid by your end customer and Qover makes sure to pay these out to the concerned, local institutions on your behalf. You therefore do not need to register yourself to or for anything.```

The **payment** of the insurance happens on your end. This means that a consumer will buy its bike + bike insurance in one go and will proceed as per usual to your checkout page with your installed payment methods (split payment methods are allowed to be used). 
Qover will provide a monthly reporting of the following:
* An invoice that you will need to pay (i.e. "reimburse") which equals the total amount of insurance contracts (premiums) sold in a given month [(Example)](https://drive.google.com/open?id=1NbGCW4sYMNfJJGnR-M4OJa-FhSLCIzl9&authuser=ines%40qover.com&usp=drive_fs). 

```Note: it is possible to automate this with a SEPA mandate - please contact your commercial SPOC should you wish to put this into place.```
* A "bordereaux" which is an overview of all sold insurance contracts and the commission you are entitled to receive for those (if applicable) in a given month [(Example)](https://drive.google.com/open?id=11MithxVnISrYOc0x5QdVk-NxBmpGstnf&authuser=ines%40qover.com&usp=drive_fs).

```Note: reverse billing is an option if you prefer to do so - please contact your commercial SPOC should you wish to put this into place.```

Since you **collect money on behalf of a third party (i.e. Qover)**, you should book it from an **accounting** point of view as a debt because you collect money that eventually doesn't belong to your company. This debt is then cleared as soon as you pay the [invoice from Qover](https://drive.google.com/file/d/1NbGCW4sYMNfJJGnR-M4OJa-FhSLCIzl9/view?usp=sharing).

## 4. Voucher flow
If you want to know how the voucher management is done, you can check it out [here](https://drive.google.com/file/d/1vX7mncK3GlvDRhYLRBvN5MEW7jjQ6yT_/view?usp=sharing).
<img width="535" alt="image" src="https://user-images.githubusercontent.com/99665011/169759285-efa900c7-3ac2-40b7-a1b7-7f29524f72be.png">

## 5. Claims process
Below you see the overview of the different steps of our claims process and how claims are handled, check it out [here](https://drive.google.com/file/d/1sCiUWn5UaaUIk-pvFmAwNxFaMrRx2UkM/view?usp=sharing).
<img width="1416" alt="image" src="https://user-images.githubusercontent.com/99665011/174753768-87a5c8e2-0774-4ea7-9c4a-4d59cea1654d.png">

## 6. Backend guide
We created a [Postman API](https://documenter.getpostman.com/view/3410894/UVRBmkmm) collection that you can copy and play with. The goal of this documentation is to give you a clear guide that can be followed when integrating the Qover API. 

Here are the generic **Qover sandbox keys** that can be used for testing if you don't have your own keys:
* **publicKey**: pk_*****
* **secretKey**: sk_*****

## 7. Post go-live
Information for your customer care team can be found in [this](https://storage.googleapis.com/qover-assets/documents/bike/Qover-bike-explanation_Ancillary-customer-care-team.pdf) documentation

## 8. Contact details
Please do not hesitate to contact us if anything is unclear on the below email addresses:
* For **commercial questions** &rarr; josephine.misson@qover.com
* For **technical questions** &rarr; product-request@qover.com
