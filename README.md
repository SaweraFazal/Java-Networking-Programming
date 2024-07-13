# Java-Networking-Programming
Develop ClientServer,GUI Chat and other apps


#getting ip from domain

import java.net.InetAddress;
import java.net.UnknownHostException;

public class main{
    public static void main(String[] args) throws UnknownHostException{
        InetAddress watcho=InetAddress.getByName("www.worthcrete.com");
        System.out.println(watcho);
    }      
}
output=>
www.worthcrete.com/104.21.84.192
=== Code Execution Successful ===


#The URLConnection class contains many methods that let you communicate with the URL over the network. URLConnection is an HTTP-centric class; that is, many of its methods are useful only when you are working with HTTP URLs. However, most URL protocols allow you to read from and write to the connection.

import java.io.BufferedReader;
import java.io.InputStreamReader;
import java.net.HttpURLConnection;
import java.net.URL;
import java.net.URLConnection;
import java.io.IOException;

public class Main{
public static void main(String[] args) throws IOException{
try{
URL url=new URL("https://www.worthcrete.com/");
URLConnection myurlConnection=url.openConnection();
BufferedReader br=new BufferedReader(new InputStreamReader(myurlConnection.getInputStream()));
String myLine;
while ((myLine=br.readLine()) !=null) {
System.out.println(myLine);
}
br.close();
}
catch(IOException exception){
System.out.println(exception.getMessage());}
}}


