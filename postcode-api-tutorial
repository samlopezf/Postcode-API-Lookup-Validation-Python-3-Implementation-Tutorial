import urllib.request as req
import json

def loadJsonResponse(url):
    return json.loads(req.urlopen(url).read())['result']

def validatePostcode(postcode):
    url = 'https://api.postcodes.io/postcodes/{}/validate'.format(postcode)
    return loadJsonResponse(url)

def randomPostcode():
    url = 'https://api.postcodes.io/random/postcodes'
    return loadJsonResponse(url)

def queryPostcode(postcode):
    url = 'https://api.postcodes.io/postcodes?q={}'.format(postcode)
    return loadJsonResponse(url)

def getAutoCompletePostcode(postcode):
    url = 'https://api.postcodes.io/postcodes/{}/autocomplete'.format(postcode)
    return loadJsonResponse(url)
