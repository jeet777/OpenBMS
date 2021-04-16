# OpenBMS
## Open Communication protocol for BMS. 
### Category:
1. Communication with Ev Charger
> * Identification
> > * Make (8 Char Code)
> > * Hardware Version (4 Char Numeric)
> > * Firmware Version (4 Char Numeric)
> > * GUID  (16 Char Alpha Numeric)
> * Parameters get/set
> > * Battery parameters 1-1000 Read only
> > * Settings 1-1000 Read/Write  
> * Precharge
> > * Precharge Init indication from EV Chareger
> > * Prcharge parameter from BMS 
> > * Precharge start ind from EVSE
> > * Precharge abort ind from EVSE
> > * Precharge complete ind from EVSE
> * PowerTransfer
> > * Charging init ind from EVSE
> > * Charging parameter from BMS (Voltage , current , power demand, charging mode CC/CV, charging allowed / not allowed) , periodic message 250ms
> > * Charging status from BMS (soc, voltage, charging current, Internal Temp max) periodic message 250ms 
> > * Charging start ind from EVSE
> > * Charging abort ind from EVSE
> > * Charging complete ind from EVSE
> * Closure
2. Communication with VCU  
> * Identification
> * Parameters get/set 
> * PowerTransfer
> * Closure
3. Dignostics (UDS) 
> * Data Transmission	
> * Stored Data Transmission	
> * Input / Output Control	
> * Upload / Download

## Base protocol  
> * ISO-TP over CAN Bus
> * Baud rate - 500 kbps
> * Fixed address 
