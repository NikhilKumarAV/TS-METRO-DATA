# TS-METRO-DATA

Hyderabad Metro Rail Data
url for datasource : https://hmrl.co.in/open-data/
download date: 07/01/2024
file date : 11/12/2023

----------------------------------------------------------------------------------------------------------------------------------------------

tables and columns and sample data (max 10 rows):

1) agency
agency_id,agency_name,agency_url,agency_timezone,agency_lang,agency_fare_url,agency_email,agency_phone

HMRL,Hyderabad Metro Rail,https://www.ltmetro.com,Asia/Kolkata,en,https://www.ltmetro.com/ticketing/,customerservice@ltmetro.com,+91-4023332555
-------------------------
2) calendar
service_id,monday,tuesday,wednesday,thursday,friday,saturday,sunday,start_date,end_date

WK,1,1,1,1,1,1,1,20231201,20300101
SA,0,0,0,0,0,1,0,20231201,20300101
SU,0,0,0,0,0,0,1,20231201,20300101
-------------------------
3) Fare attributes
fare_id,price,currency_type,payment_method,transfers,agency_id

F_10,10,INR,1,,HMRL
F_15,15,INR,1,,HMRL
F_25,25,INR,1,,HMRL
F_30,30,INR,1,,HMRL
F_35,35,INR,1,,HMRL
F_40,40,INR,1,,HMRL
F_45,45,INR,1,,HMRL
F_50,50,INR,1,,HMRL
F_55,55,INR,1,,HMRL
F_60,60,INR,1,,HMRL
-------------------------
4) fare_rules
origin_id,destination_id,fare_id

NAG,NAG,F_10
UPL,NAG,F_10
STD,NAG,F_15
NGR,NAG,F_15
HSG,NAG,F_25
TAR,NAG,F_25
MET,NAG,F_30
SEC_E,NAG,F_35
PRG,NAG,F_40
PAR,NAG,F_40
-------------------------
5) routes
route_id,agency_id,route_short_name,route_long_name,route_type,route_color,route_text_color,route_sort_order

RED,HMRL,C1_RED,Miyapur - LB Nagar - Miyapur - C1,1,E31E24,FFFFFF,1
GREEN,HMRL,C2_GREEN,JBS Parade Ground - MG Bus Station - JBS Parade Ground - C2,1,009846,000000,2
BLUE,HMRL,C3_BLUE,Nagole - Raidurg - Nagole - C3,1,007ABB,000000,3
-------------------------
6) stop_times
trip_id,stop_sequence,stop_id,arrival_time,departure_time,timepoint

SA_100585,1,RDG2,07:32:29,07:33:55,1
SA_100585,2,HTC2,07:36:36,07:36:51,1
SA_100585,3,DGC2,07:38:09,07:38:24,1
SA_100585,4,MAD2,07:40:47,07:41:02,1
SA_100585,5,PED2,07:42:57,07:43:12,1
SA_100585,6,JCP2,07:44:34,07:44:49,1
SA_100585,7,JR52,07:46:57,07:47:12,1
SA_100585,8,YUG2,07:48:45,07:49:00,1
SA_100585,9,MUN2,07:51:17,07:51:32,1
SA_100585,10,AME2,07:52:59,07:53:44,1
-------------------------
7) stops
stop_id,stop_name,stop_lat,stop_lon,zone_id,location_type,parent_station,platform_code

MYP,Miyapur,17.4965452,78.3730262,MYP,1,,
MYP1,Miyapur,17.4965452,78.3730262,MYP,0,MYP,1
MYP2,Miyapur,17.4965452,78.3730262,MYP,0,MYP,2
JNT,JNTU College,17.4987037,78.3888668,JNT,1,,
JNT1,JNTU College,17.4987037,78.3888668,JNT,0,JNT,1
JNT2,JNTU College,17.4987037,78.3888668,JNT,0,JNT,2
KPH,KPHB Colony,17.4937602,78.4018258,KPH,1,,
KPH1,KPHB Colony,17.4937602,78.4018258,KPH,0,KPH,1
KPH2,KPHB Colony,17.4937602,78.4018258,KPH,0,KPH,2
KUK,Kukatpally,17.4849033,78.4117896,KUK,1,,
-------------------------
8)trips
service_id,route_id,trip_id,direction_id,trip_headsign,block_id

SA,BLUE,SA_100585,1,Nagole,SA_30201
SA,BLUE,SA_100586,0,Raidurg,SA_31401
SA,BLUE,SA_100587,1,Nagole,SA_31401
SA,BLUE,SA_100588,0,Raidurg,SA_30601
SA,BLUE,SA_100589,1,Nagole,SA_30601
SA,BLUE,SA_100590,0,Raidurg,SA_31501
SA,BLUE,SA_100591,1,Nagole,SA_31501
SA,BLUE,SA_100592,0,Raidurg,SA_30701
SA,BLUE,SA_100593,1,Nagole,SA_30701
SA,BLUE,SA_100594,0,Raidurg,SA_31601

------------------------------------------------------------------------------------------------------------------------------




