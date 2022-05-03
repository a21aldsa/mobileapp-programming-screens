
# Rapport

Jag forkade projektet från github
sedan skapade jag en andra activity och döpte den till SecondActivity
sedan skapade jag en knapp i activity_main
jag skapade en intent som öppar min andra activity, jag gav den även extras i form av namn(Halloj)och nummer(50)
sedan satte jag intenten inom en onclick för knappen
min onclick ser ut så här:
```
Button button = findViewById(R.id.mainButton);
button.setOnClickListener(new View.OnClickListener() {
    @Override
    public void onClick(View view) {
        Intent intent = new Intent(MainActivity.this, SecondActivity.class);
        intent.putExtra("name", "Halloj");
        intent.putExtra("number", 50);
        startActivity(intent);
    }
});
```
sedan satte jag handlers i SecondActivity som hanterade extras från MainActivity

![](android.png)