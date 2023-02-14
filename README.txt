################################################################
TITLE: OBLABS REST API
AUTOR: obarrientos
DATE: 02/13/2023
NOTES: Spring Boot | MySQL | OAuth2
################################################################


SERVICES AVAILABLE IN THIS API
----------------------------------------------------------------
LOGIN(string:user, string:password)
LOG_SESSION(string:Token);
AUTHENTICATE(string:Token, string:User);
CREATE_USER(string:Username,string:Password,string:Email,string:FirstName,string:MiddleName,string:LastName,string:DOB,string:SSN,string:Address_1,string:Address_2, string:city,string:state,string:zip, string:country,string:geo_long,string:geo_lat, string:ip_address, string:mac_address, string:device_id, string:serial, string:OS,string:internet_provider, string:google_address);
UPDATE_USER(int:Id,string:Username,string:Password,string:Email,string:FirstName,string:MiddleName,string:LastName,string:DOB,string:SSN,string:Address_1,string:Address_2, string:city,string:state,string:zip, string:country,string:geo_long,string:geo_lat, string:ip_address, string:mac_address, string:device_id, string:serial, string:OS,string:internet_provider, string:google_address );
DELETE_USER(int:Id);
SEARCH_USER_BY_ID(int:Id);
SEARCH_USERS(string:Search_Param);
DELETE_ALL_USERS(string:Search_Param);
CREATE_ROLE(int:Id,string:name,string:Name,string:Description);
UPDATE_ROLE(int:Id);
SEARCH_ROLE_BY_ID(int:Id);
SEARCH_ROLES(string:Search_Param);
DELETE ROLE(int:Id);
ASSIGN_ROLE(int:UserId, int:RoleId);
CREATE_LIST(int:Id,string:Name,string:Description);
UPDATE_LIST(int:Id);
DELETE_LIST(int:Id);
SEARCH_LIST_BY_ID(int:Id);
SEARCH_LISTS(string:Search_Param);
CREATE_LIST_VALUE(int:Id,string:Name,string:Description);
UPDATE_LIST_VALUE(int:Id);
DELETE_LIST_VALUE(int:Id);
SEARCH_LIST_VALUE_ID(int:Id);
SEARCH_LIST_VALUES(int:ListID,string:Search_Param);
UPLOAD_DOCUMENT(int:Id, object:File);


################################################################