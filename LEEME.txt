[Actualizacion 03/08/2021]

Esto sera la explicacion con el primer cliente que tenemos
guardado en natural_clients

//EJEMPLO - EJEMPLO - EJEMPLO//

	"25033578": {
        "accounts": [],
		"phone": 3200722812,
        "client_name": "Curtis Archer",
        "client_occupation": "estudiante",
        "client_address": "339 Lauren Avenue Williamsonborough, OR 84368"
	}

//EJEMPLO - EJEMPLO - EJEMPLO//
//EXPLICACION - EXPLICACION - EXPLICACION//

	"client_id": {						//Este es el client_id para los clientes naturales es su Cedula
		"accounts" [Strings Array],		//Aqui se escriben los id de las cuentas que corresponden a este cliente
		"phone": "String",				//LOS TELEFONOS DEBEN SER STRINGS
		"client_name": "String",		//El nombre del dueño de la cuenta
		"client_occupation": "String",	//En que trabaja este cliente
		"client_address": "String",		//La direccion del cliente
	}

//EXPLICACION - EXPLICACION - EXPLICACION//

Esto sera la explicacion con el primer cliente que tenemos
guardado en company_clients

//EJEMPLO - EJEMPLO - EJEMPLO//

	"35559562-1": {
       	"accounts": [],
	    "phone": 3181608631,
      	"client_name": "Joshua Powell",
	    "client_occupation": "cajero",
	    "client_address": "0096 David Meadows Suite 231 Brookeborough, CO 43491",
	    "client_id": "35559562",
      	"company_name": "Pan Diaz",
	    "cluster": "internet"
    }

//EJEMPLO - EJEMPLO - EJEMPLO//
//EXPLICACION - EXPLICACION - EXPLICACION//

	"nit": {							//Este es el nit de la empresa, generalmente es su Cedula seguido de un guion y un numero de confirmacion
        "accounts" [Strings Array],		//Aqui se escriben los id de las cuentas que corresponden a este cliente
	    "phone": "String",				//LOS TELEFONOS DEBEN SER STRINGS
		"client_name": "String",		//El nombre del dueño de la cuenta
		"client_occupation": "String",	//En que trabaja este cliente
		"client_address": "String",		//La direccion del cliente
	    "client_id": "35559562",		//La cedula del dueño legal de esta cuenta
        "company_name": "Pan Diaz",		//Nombre de la compañia
	    "cluster": "internet"			//Sector laboral de la compañia
    }

//EXPLICACION - EXPLICACION - EXPLICACION//

Esta es una explicacion de una cuenta X guardada en saving-accounts.json
o en current-accounts.json

//EJEMPLO - EJEMPLO - EJEMPLO//

	"99900025": {
		"client_id": "25033578",
		"balance": 250250000,
		"isActive": true,
		"suc_id": "2",
		"transactions": ["352352-T"],
		"creation_date": "08-08-2016"
	}

//EJEMPLO - EJEMPLO - EJEMPLO//
//EXPLICACION - EXPLICACION - EXPLICACION//

	"account_id": {							//ID unico de la cuenta
		"client_id": "25033578",			//ID del cliente al que pertenece esta cuenta
		"balance": Float,					//Dinero dentro de la cuenta
		"isActive": Boolean,				//Booleando que nos indica si la cuenta esta activa o no
		"suc_id": "String",					//id de la sucursal donde se creo esta cuenta
		"transactions": [Strings Array],	//Array de Strings donde estan los id de las transaciones que a tenido esta cuenta
		"creation_date": "Date"				//Dato tipo Date con la fecha de creacion de la cuenta
	}

//EXPLICACION - EXPLICACION - EXPLICACION//

Esta es la explicacion de los primeros 3 cajeros en cashiers.json

//EJEMPLO - EJEMPLO - EJEMPLO//

	"0": {
        "sucursal_id": "0"
    },
    "1": {
        "sucursal_id": "0"
    },
    "2": {
        "sucursal_id": "4"
    }
	
//EJEMPLO - EJEMPLO - EJEMPLO//
//EXPLICACION - EXPLICACION - EXPLICACION//

	"cashier_id": {					//Aqui se escribe el id unico de este cajero
		"sucursal_id": "String"		//Aqui se escribe la id unica de la sucursal a la que pertenece este cajero
	}
	
//EXPLICACION - EXPLICACION - EXPLICACION//

Esta es la explicacion de las primeras 2 sucursales guardadas en sucursals.json

//EJEMPLO - EJEMPLO - EJEMPLO//

	"0": {
        "cashiers": [
            "0",
            "1",
            "18",
            "20",
            "26",
            "33",
            "34",
            "41"
        ],
        "sucursal_address": "50932 Williams Locks Johnsonchester, PA 18261",
        "city": "pereira"
    },
    "1": {
        "cashiers": [
            "37",
            "45"
        ],
        "sucursal_address": "3484 Flores Mission Apt. 641 Kevinberg, AZ 74783",
        "city": "medellin"
    }
	
//EJEMPLO - EJEMPLO - EJEMPLO//
//EXPLICACION - EXPLICACION - EXPLICACION//

	"sucursal_id": {						//id de identificacion unico de esta sucursal
		"cashiers": [						//array de Strings
			"cashier_id"					//id de identificacion unico de este cajero
			"cashier_id"					//"
			"cashier_id"
			"cashier_id"
		],
		"sucursal_address": "String",		//direccion de la sucursal
		"city": "String"					//ciudad donde esta ubicada la sucursal
	}
	
//EXPLICACION - EXPLICACION - EXPLICACION//

Por ultimo el JSON con las transaciones

//EJEMPLO - EJEMPLO - EJEMPLO//

	"46465-C": {
		"transaction_name": "Consignacion",
		"cashier_id": "Cajero 12",
		"to_account_id": "98035022",
		"value": "250000",
		"transaction_date": "04-08-2021",
		"sucursal_id": "3",
	},
	
	"35552-R": {
		"transaction_name": "Retiro",
		"from_account_id": "99900025",
		"value": "14000",
		"transaction_date": "02-08-2021",
		"sucursal_id": "2"
	}
	
//EJEMPLO - EJEMPLO - EJEMPLO//
//EXPLICACION - EXPLICACION - EXPLICACION//

	"transaction_id": {						//id de identificacion unico para esta transacion adicional a su identificador [C - R - T - X]
		"transaction_name": "String",		//nombre de la transacion
		"from_account_id": "String",		//OPCIONAL id de la cuenta desde donde se realiza la transacion
		"to_account_id": "String",			//OPCIONAL id de la cuenta objetivo de la transacion
		"value": Float,						//valor de la transacion
		"transaction_date": Date,			//fecha de la transacion
		"sucursal_id": "String"				//id unico de identificacion donde se realiza la transacion
	}
	
//EXPLICACION - EXPLICACION - EXPLICACION//