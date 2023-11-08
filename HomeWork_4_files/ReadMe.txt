public class HomeWork_4 {
//აქ გამოვიყენე class- ი
    @Test
    public void searchInput(){
        open("https://www.google.com/");
        $(".gLFyf").click();
    }

აქაც გამოვიყენე class- ი, ID - ით მინდოდა მაგრამ ვერ ვიპოვე:D, სერჩ ბარში ტექსტის გარეშე ტესტი მიფეილდებოდა  და მიწერდა element should be clickable:, ამიტომ დავამატე ტექსტის ჩაწერა და ტესტი აღარ დაფეილდა,
    @Test
    public void googleSearchButton(){
        open("https://www.google.com/");
        $(".gLFyf").setValue("Automated Testing with Selenide");
        $(".gNO89b").click();
    }

//ესეც xpath
    @Test
    public void images(){
        open("https://www.google.com/");
        $(By.xpath("//*[@id=\"gb\"]/div/div[1]/div/div[2]/a")).click();

    }
}
