# ios
ios
int main(int argc, const char * argv[]) {
   
    int y,m,d;
    printf("输入年:");
    scanf("%d",&y);
    while(y > 2015)
    {
        
        printf("年份不合法,请重新输入年:\n");
        scanf("%d",&y);
        
    }
    printf("输入月:");
    scanf("%d",&m);
    while(m > 12)
    {
        
        printf("月份不合法,请重新输入月:\n");
        scanf("%d",&m);
        
    }

    printf("输入日:");
    scanf("%d",&d);
    while (d > 31)
   {
      printf("日不合法,请重新输入日:\n");
      scanf("%d",&d);
    }
    
    switch (m) {
        case 2:
        {
            if((y % 4 ==0 && y %100 !=0)||y%400==0)
            {
                while(d > 29)
                {
                    printf("日不合法,请从新输入:");
                    scanf("%d",&d);
                }
            }
            else
            {
                while(d > 28)
                {
                    printf("日不合法,请从新输入:");
                    scanf("%d",&d);
                }
            }
            
            
        }
            break;
            case 4:
            {
                while (d > 30)
                {
                    printf("日不合法,请从新输入:");
                    scanf("%d",&d);
                }
            
            }
            break;
        case 6:
        {
            while (d > 30)
            {
                printf("日不合法,请从新输入:");
                scanf("%d",&d);
            }
            
        }
            break;
        case 9:
        {
            while (d > 30)
            {
                printf("日不合法,请从新输入:");
                scanf("%d",&d);
            }
            
        }
            break;
        case 11:
        {
            while (d > 30)
            {
                printf("日不合法,请从新输入:");
                scanf("%d",&d);
            }
            
        }
            break;

        default:
            break;
    }
    
    
    printf("您输入的生日合法.\n");
    printf("您的生日是:%d年%d月%d日.\n",y,m,d);
    
    
    
    
