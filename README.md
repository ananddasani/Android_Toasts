# Android_Toasts
See the All types of Toasts in Android

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

<img src="app_images/All Toast Code.png" width="1000" /><br>

<img src="app_images/All Toast App1.png" width="300" /><br>

<img src="app_images/All Toast App2.png" width="300" /><br>

<img src="app_images/All Toast App3.png" width="300" /><br>
