import java.text.SimpleDateFormat;
import java.util.Calendar;

import org.openqa.selenium.remote.RemoteWebDriver;
import org.testng.annotations.Test;
import org.testng.xml.XmlTest;

import com.omniwyse.selenium.data.DataManager;

public class EfareTest {

	RemoteWebDriver driver;

	@Test
	public void f(XmlTest config) throws Exception {
		DataManager.config = config;
		String repositoryPath = "D:\\oWyseTestBase\\";
		DataManager.currentDate = new SimpleDateFormat("dd-MM-yyyy").format(Calendar.getInstance().getTime());
		DataManager.timestamp=new SimpleDateFormat("HH_mm_ss").format(Calendar.getInstance().getTime());
		System.out.println(DataManager.currentDate);
		System.out.println("this is our repository path " + repositoryPath);
		//Files.createDirectories(Paths.get("D:\\oWyseTestBase\\Results\\"+DataManager.currentDate));//stmt for creating folder dynamically...
		new DataManager().executeTestPlan(repositoryPath, DataManager.currentDate);
		System.out.println("Input(TestPlan) file reading is done..");
	}
}
