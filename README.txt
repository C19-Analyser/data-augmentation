DATA AUGMENTATION :

D.A. V1 -> image augmented pour une seule image

D.A. V2 -> dossier augmented pour un dossier d'image

scratch_10G_AUGMENTED.h5 -> "MODEL" enregistré avec la data augmentation la plus probablement optimisé (95%)
        rotation_range=45,     #Borne de la rotation donc de 0 a 45
        width_shift_range=0.2,   #Borne du deplacement sur X
        height_shift_range=0.2, #Borne du deplacement sur Y
        shear_range=0.2,     #ça je suis pas sur shear = depouiller tondre
        zoom_range=0.2, #Borne du zoom qu'on va appliquer a notre image
        horizontal_flip=True, #ça c'est pour flip a l'horizontale classico del madrido
        fill_mode='constant'
        
scratch_10G_AUGMENTED2.h5 -> "MODEL" enregistré avec la data augmentation (75%)      
        rotation_range=90,     #Borne de la rotation donc de 0 a 45
        width_shift_range=0.5,   #Borne du deplacement sur X
        height_shift_range=0.5, #Borne du deplacement sur Y
        shear_range=0.5,     #ça je suis pas sur shear = depouiller tondre
        zoom_range=0.5, #Borne du zoom qu'on va appliquer a notre image
        horizontal_flip=True, #ça c'est pour flip a l'horizontale classico del madrido
        fill_mode='constant'
        
scratch_10G_AUGMENTED3.h5 -> "MODEL" enregistré avec la data augmentation (95%)
        rotation_range=20,
        zoom_range=0.15,
        width_shift_range=0.2,
        height_shift_range=0.2,
        shear_range=0.15,
        horizontal_flip=True,
        fill_mode="nearest"
