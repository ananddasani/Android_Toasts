# Android_Toasts
See the All types of Toasts in Android

This topic is a part of [My Complete Andorid Course](https://github.com/ananddasani/Android_Apps)

# Code

#### MainActivity.java
```
Button default_toast, gravity_toast, nestedGravity_toast;
  
//list the items
default_toast = findViewById(R.id.simple);
gravity_toast = findViewById(R.id.gravity);
nestedGravity_toast = findViewById(R.id.nestedGravity);

//set on click listener
default_toast.setOnClickListener(this);
gravity_toast.setOnClickListener(this);
nestedGravity_toast.setOnClickListener(this);

    @Override
    public void onClick(View v) {

        switch (v.getId()){
            case R.id.simple:
                Toast.makeText(this, "This is a Default Toast", Toast.LENGTH_SHORT).show();
                break;

            case R.id.gravity:
                Toast toast = Toast.makeText(this, "This is Gravity Toast", Toast.LENGTH_LONG);
                toast.setGravity(Gravity.CENTER, 100, 100);
                toast.show();
                break;

            case R.id.nestedGravity:
                Toast toast1 = Toast.makeText(this, "This is a Nested Gravity Toast", Toast.LENGTH_LONG);
                toast1.setGravity(Gravity.BOTTOM | Gravity.RIGHT, 0, 0);
                toast1.show();
                break;
        }
    }
```

# App Highlight

![All Toast App1](https://user-images.githubusercontent.com/74413402/192092681-3d154c4c-bfeb-41e1-b302-20feb89f9b6f.png)
![All Toast App2](https://user-images.githubusercontent.com/74413402/192092683-536fb1ed-8e0d-4d5c-8541-de2af6102949.png)
![All Toast App3](https://user-images.githubusercontent.com/74413402/192092684-2cb2c713-867d-4324-9988-37e5f3674f1d.png)
![All Toasts Code](https://user-images.githubusercontent.com/74413402/192092685-e1b5bb50-5130-4041-8f8c-31847f8f712f.png)
