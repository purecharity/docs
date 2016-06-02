#### Fundraiser API

###### GET external_fundraisers/

Returns a collection of fundraisers along with the current page and the total number pages.

**Optional Parameters**

- campaign_id: Returns only the fundraisers where the campaign_id matches with this parameter
- dir: The sort order (default: “desc”)
- sort: The sortable field (date, name, last_name, founder)
- page: The page number (default: 1)
- limit: The number of entries per page (default: 100)

Example Result:

```
{
  "external_fundraisers": [
    {
      "id": 3,
      "name": "Kitties Unite!",
      "slug": "kitties-unite",
      "about": "We want to organize a gathering of cats for everyone to get to enjoy their cuteness.",
      "region": null,
      "country": "United States",
      "field_partner_id": 1,
      "start_date": "2015-03-27T03:00:00Z",
      "end_date": "2016-03-27T03:00:00Z",
      "images": {
        "large": "http://purecharity.com/uploads/profile/cover_photo/46/image.jpeg",
        "medium": null,
        "small": "http://purecharity.com/uploads/avatar/image/45/image.jpg"
      },
      "public_url": "http://purecharity.com/kitties-unite",
      "funding_goal": 50000,
      "funding_needed": 49927,
      "recurring_funding_goal": 2000,
      "owner": {
        "name": "John Cleese",
        "slug": "johncleese",
        "avatar": "http://purecharity.com/uploads/avatar/image/4/image.png",
        "profile": {
          "cover_photo": {
            "url": "/images/avatar_defaults/image.png",
            "cover": {
              "url": "/images/avatar_defaults/image.png"
            },
            "photo": {
              "url": "/images/avatar_defaults/image.png"
            },
            "widget": {
              "url": "/images/avatar_defaults/image.png"
            },
            "small": {
              "url": "/images/avatar_defaults/image.png"
            }
          }
        }
      },
      "category": {
        "name": "Food",
        "description": "Eradicate extreme hunger and improve basic nutrition."
      }
    },
    {
      "id": 1,
      "name": "Teens United To Change the World",
      "slug": "teens-united-to-change-the-world",
      "about": "Join the movement of teens who are taking a stand to change the world!",
      "region": null,
      "country": "United States",
      "field_partner_id": 1,
      "start_date": "2015-03-27T03:00:00Z",
      "end_date": "2016-03-27T03:00:00Z",
      "images": {
        "large": "http://purecharity.com/uploads/profile/cover_photo/44/image.jpg",
        "medium": null,
        "small": "http://purecharity.com/uploads/avatar/image/43/image.jpg"
      },
      "public_url": "http://purecharity.com/teens-united-to-change-the-world",
      "funding_goal": 500000,
      "funding_needed": 306398,
      "recurring_funding_goal": null,
      "owner": {
        "name": "Charity",
        "slug": "charity",
        "avatar": "http://purecharity.com/uploads/avatar/image/18/image.jpg",
        "profile": {
          "cover_photo": {
            "url": "http://purecharity.com/uploads/profile/cover_photo/19/image.jpg",
            "cover": {
              "url": "http://purecharity.com/uploads/profile/cover_photo/19/cover_image.jpg"
            },
            "photo": {
              "url": "http://purecharity.com/uploads/profile/cover_photo/19/photo_image.jpg"
            },
            "widget": {
              "url": "http://purecharity.com/uploads/profile/cover_photo/19/widget_image.jpg"
            },
            "small": {
              "url": "http://purecharity.com/uploads/profile/cover_photo/19/small_image.jpg"
            }
          }
        }
      },
      "category": {
        "name": "Opportunity",
        "description": "Education, homeless services, job creation, orphan care, and other efforts to end extreme poverty."
      }
    }
  ],
  "meta": {
    "current_page": 1,
    "num_pages": 9
  }
}
```

###### GET external_fundraisers/:id

Returns an individual fundraiser's settings and content.

Example result:

```
{
  "fundraiser": {
    "id": 1,
    "name": "Teens United To Change the World",
    "slug": "teens-united-to-change-the-world",
    "about": "Join the movement of teens who are taking a stand to change the world.  We're giving our voice and money to end modern day slavery for the 27 million people in bondage, feeding our brothers and sisters in need and delivering hope to the world. It's time to rise up, be counted and join the movement to eliminate these injustices in our generation!",
    "region": null,
    "country": "United States",
    "field_partner_id": 1,
    "funding_goal": 500000,
    "funding_needed": 306398,
    "recurring_funding_goal": null,
    "start_date": "2015-03-27T03:00:00Z",
    "end_date": "2016-03-27T03:00:00Z",
    "images": {
      "large": "http://purecharity.com/uploads/profile/cover_photo/44/orphan4.jpg",
      "medium": null,
      "small": "http://purecharity.com/uploads/avatar/image/43/DSC_8408_20avatar.jpg"
    },
    "fundraiser_type": "birthday",
    "updates": [
      {
        "title": "Sample update number 6 for Teens United To Change the World ",
        "body": "Lorem ipsum dolor sit amet,\nAenean massa. Cum sociis natoque penatibus et magnis\ndis parturient montes, nascetur ridiculus mus. ",
        "author": {
          "name": "James Bond",
          "slug": "james-bond",
          "avatar": "http://purecharity.com/uploads/avatar/image/1/image.jpg",
          "profile": {
            "cover_photo": {
              "url": "http://purecharity.com/images/avatar_defaults/image.png",
              "cover": {
                "url": "http://purecharity.com/images/avatar_defaults/image.png"
              },
              "photo": {
                "url": "http://purecharity.com/images/avatar_defaults/image.png"
              },
              "widget": {
                "url": "http://purecharity.com/images/avatar_defaults/image.png"
              },
              "small": {
                "url": "http://purecharity.com/images/avatar_defaults/image.png"
              }
            }
          }
        },
        "url": "http://purecharity.com/teens-united-to-change-the-world/updates/8"
      }
    ],
    "embed_code": "",
    "owner": {
      "name": "Charity",
      "slug": "charity",
      "avatar": "http://purecharity.com/uploads/avatar/image/18/image.jpg",
      "profile": {
        "cover_photo": {
          "url": "http://purecharity.com/uploads/profile/cover_photo/19/image.jpg",
          "cover": {
            "url": "http://purecharity.com/uploads/profile/cover_photo/19/cover_image.jpg"
          },
          "photo": {
            "url": "http://purecharity.com/uploads/profile/cover_photo/19/photo_image.jpg"
          },
          "widget": {
            "url": "http://purecharity.com/uploads/profile/cover_photo/19/widget_image.jpg"
          },
          "small": {
            "url": "http://purecharity.com/uploads/profile/cover_photo/19/small_image.jpg"
          }
        }
      }
    },
    "category": {
      "name": "Opportunity",
      "description": "Education, homeless services, job creation, orphan care, and other efforts to end extreme poverty."
    },
    "field_partner": {
      "name": "Teen Mania Ministries",
      "slug": "teen-mania",
      "avatar": "http://purecharity.com/uploads/avatar/image/17/image.png",
      "profile": {
        "cover_photo": {
          "url": "http://purecharity.com/uploads/profile/cover_photo/18/image.JPG",
          "cover": {
            "url": "http://purecharity.com/uploads/profile/cover_photo/18/cover_image.JPG"
          },
          "photo": {
            "url": "http://purecharity.com/uploads/profile/cover_photo/18/photo_image.JPG"
          },
          "widget": {
            "url": "http://purecharity.com/uploads/profile/cover_photo/18/widget_image.JPG"
          },
          "small": {
            "url": "http://purecharity.com/uploads/profile/cover_photo/18/small_image.JPG"
          }
        }
      }
    },
    "backers": [
      {
        "name": "James Bond",
        "slug": "james-bond",
        "avatar": "http://purecharity.com/uploads/avatar/image/1/image.jpg",
        "profile": {
          "cover_photo": {
            "url": "http://purecharity.com/images/avatar_defaults/image.png",
            "cover": {
              "url": "http://purecharity.com/images/avatar_defaults/image.png"
            },
            "photo": {
              "url": "http://purecharity.com/images/avatar_defaults/image.png"
            },
            "widget": {
              "url": "http://purecharity.com/images/avatar_defaults/image.png"
            },
            "small": {
              "url": "http://purecharity.com/images/avatar_defaults/image.png"
            }
          }
        }
      },
      {
        "name": "John Smith",
        "slug": "johnsmith",
        "avatar": "http://purecharity.com/uploads/avatar/image/6/image.png",
        "profile": {
          "cover_photo": {
            "url": "http://purecharity.com/images/avatar_defaults/image.png",
            "cover": {
              "url": "http://purecharity.com/images/avatar_defaults/image.png"
            },
            "photo": {
              "url": "http://purecharity.com/images/avatar_defaults/image.png"
            },
            "widget": {
              "url": "http://purecharity.com/images/avatar_defaults/image.png"
            },
            "small": {
              "url": "http://purecharity.com/images/avatar_defaults/image.png"
            }
          }
        }
      },
      {
        "name": "Peter Giver",
        "slug": "petergiver",
        "avatar": "http://purecharity.com/uploads/avatar/image/5/image.jpeg",
        "profile": {
          "cover_photo": {
            "url": "http://purecharity.com/images/avatar_defaults/image.png",
            "cover": {
              "url": "http://purecharity.com/images/avatar_defaults/image.png"
            },
            "photo": {
              "url": "http://purecharity.com/images/avatar_defaults/image.png"
            },
            "widget": {
              "url": "http://purecharity.com/images/avatar_defaults/image.png"
            },
            "small": {
              "url": "http://purecharity.com/images/avatar_defaults/image.png"
            }
          }
        }
      }
    ]
  }
}
```

