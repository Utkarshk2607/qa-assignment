# qa-assignment
import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.chrome.ChromeDriver;

public class techwondoe {
	public static void main(String[] args) throws InterruptedException  {
		    System.setProperty("webdriver.chrome.driver", "C:\\Users\\HP\\Downloads\\chromedriver_win32\\chromedriver.exe");
			WebDriver driver=new ChromeDriver();
			driver.get("https://github.com/login");
			Thread.sleep(300);
			WebElement user_name=driver.findElement(By.xpath("//input[@id='login_field']"));
			user_name.sendKeys("utkarshkonarde123@gmail.com");
			Thread.sleep(300);
			WebElement password=driver.findElement(By.xpath("//input[@id='password']"));
			password.sendKeys("***********");
			Thread.sleep(300);
			WebElement login=driver.findElement(By.xpath("//input[@type='submit']"));
			login.click();
			Thread.sleep(15000);
			WebElement submit=driver.findElement(By.xpath("//button[@type='submit']"));
			submit.click();
			Thread.sleep(300);
			/*WebElement submit=driver.findElement(By.xpath("//button[@type='submit']"));
			submit.click();*/
			WebElement creat_new_repository=driver.findElement(By.xpath("//a[text()='Create a new repository']"));
			creat_new_repository.click();
			Thread.sleep(300);
			WebElement Repository_name=driver.findElement(By.xpath("//input[@name='repository[name]']"));
			Repository_name.sendKeys("Qa-assignment1");
			Thread.sleep(300);
			WebElement Add_a_README_file=driver.findElement(By.xpath("//input[@type='checkbox']"));
			Add_a_README_file.click();
			Thread.sleep(300);
			WebElement node=driver.findElement(By.xpath("//span[text()='None']"));
			node.click();
			Thread.sleep(300);
			WebElement Type=driver.findElement(By.xpath("//input[@placeholder='Filter...']"));
			Type.sendKeys("Node");
			Thread.sleep(300);
			WebElement click=driver.findElement(By.xpath("(//label[@class='SelectMenu-item text-normal'])[72]"));
			/*(//label[@class='SelectMenu-item text-normal'])[72]*/
			click.click();
			Thread.sleep(300);
			click.click();
			Thread.sleep(300);
			WebElement create_repository=driver.findElement(By.xpath("//button[@class='btn-primary btn']"));
			create_repository.click();
			Thread.sleep(300);
			WebElement profile=driver.findElement(By.xpath("//img[@alt='@Utkarshk2607']"));
			profile.click();
			Thread.sleep(300);
			WebElement logout=driver.findElement(By.xpath("//button[@class='dropdown-item dropdown-signout']"));
			logout.click();
	
		
			
		
	}
}
