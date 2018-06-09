 @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
    }
     @Override
   protected void onPause() {
        super.onPause();
        Log.e("MainActivity","onPause() is invoked！");
     }


    @Override
         protected void onResume() {
                super.onResume();
                 Log.e("MainActivity","onResume() is invoked！");
             }


    @Override
        protected void onStart() {
                 super.onStart();
             Log.e("MainActivity","onStart() is invoked！");
           }

    @Override
        protected void onRestart() {
                super.onRestart();
               Log.e("MainActivity","onRestart() is invoked！");
           }


    @Override
        protected void onStop(){
               super.onStop();
              Log.e("MainActivity","OnStop() is invoked!");
           }

}

