import java.util.*;
import java.io.*;
import java.awt.*;
import javax.imageio.ImageIO;
import javax.swing.JFrame;
import java.awt.image.BufferedImage;

class getpixel extends Canvas
{
    getpixel()
    {
        BufferedImage image;
        File f=null;
        try
        {
            f=new File("CO1.jpg");
            image=ImageIO.read(f);
            int width=image.getWidth();
            int height=image.getHeight();
            int p=image.getRGB(0,0);
            int boo=p|0xff;
            for(int i=0;i<height/2;i++)
            {
                for(int j=0;j<width/2;j++)
                {
                    image.setRGB(j,i,0xFFA500);
                }
            }
            int rgb = image.getRGB(0,0);
            int r = (rgb >> 16) & 0xFF;
            int g = (rgb >> 8) & 0xFF;
            int b = (rgb & 0xFF);
            Color c=new Color(image.getRGB(0,0));
            System.out.println("Color c : "+c.getRed()+" "+c.getBlue()+" "+c.getGreen());
            System.out.println("Int red "+r);
            System.out.println("Int green "+g);
            System.out.println("Int blue "+b);
            System.out.println("RGB is "+rgb);
            image.setRGB(0,0,rgb);
            File f1=new File("CO1.jpg");
            ImageIO.write(image, "jpg", f1);
            
            System.out.println("That was r ");
            System.out.println("Now r tried to change");
            int rr=r&0x1;
            System.out.println(r);
        }
        catch(Exception e)
        {
            System.out.println(e);
        }
    }
    public static void main(String args[])
    {
        getpixel P=new getpixel();
    }
}
            
