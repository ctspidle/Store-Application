# Store-Application
Store Class CS II 2017
        Scanner sc = new Scanner(System.in);
        Store first = new Store();
        String operation = sc.nextLine();
        if (operation.toLowerCase().equals("add item"))
        {
            first.addItem();
            System.out.println("What item would you like to add?");
            String n = sc.nextLine();
            System.out.println("Enter the type of " + n);
            String q = sc.nextLine();
            System.out.println("Enter the number of " + n + " in stock");
            int num = sc.nextInt();
            System.out.println("Enter the true cost of one " + n);
            double cost = sc.nextDouble();
            System.out.println("Enter the price of one " + n);
            double price = sc.nextDouble();
            int place = first.getItemCount()-1;
            first.setItemName(place, n);
            first.setItemType(place, q);
            first.setItemStock(place, num);
            first.setItemCost(place, cost);
            first.setItemPrice(place, price);    
        }
